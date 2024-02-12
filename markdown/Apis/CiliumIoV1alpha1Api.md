# CiliumIoV1alpha1Api

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**](CiliumIoV1alpha1Api.md#createCiliumIoV1alpha1NamespacedTracingPolicyNamespaced) | **POST** /apis/cilium.io/v1alpha1/namespaces/{namespace}/tracingpoliciesnamespaced |  |
| [**createCiliumIoV1alpha1TracingPolicy**](CiliumIoV1alpha1Api.md#createCiliumIoV1alpha1TracingPolicy) | **POST** /apis/cilium.io/v1alpha1/tracingpolicies |  |
| [**deleteCiliumIoV1alpha1CollectionNamespacedTracingPolicyNamespaced**](CiliumIoV1alpha1Api.md#deleteCiliumIoV1alpha1CollectionNamespacedTracingPolicyNamespaced) | **DELETE** /apis/cilium.io/v1alpha1/namespaces/{namespace}/tracingpoliciesnamespaced |  |
| [**deleteCiliumIoV1alpha1CollectionTracingPolicy**](CiliumIoV1alpha1Api.md#deleteCiliumIoV1alpha1CollectionTracingPolicy) | **DELETE** /apis/cilium.io/v1alpha1/tracingpolicies |  |
| [**deleteCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**](CiliumIoV1alpha1Api.md#deleteCiliumIoV1alpha1NamespacedTracingPolicyNamespaced) | **DELETE** /apis/cilium.io/v1alpha1/namespaces/{namespace}/tracingpoliciesnamespaced/{name} |  |
| [**deleteCiliumIoV1alpha1TracingPolicy**](CiliumIoV1alpha1Api.md#deleteCiliumIoV1alpha1TracingPolicy) | **DELETE** /apis/cilium.io/v1alpha1/tracingpolicies/{name} |  |
| [**listCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**](CiliumIoV1alpha1Api.md#listCiliumIoV1alpha1NamespacedTracingPolicyNamespaced) | **GET** /apis/cilium.io/v1alpha1/namespaces/{namespace}/tracingpoliciesnamespaced |  |
| [**listCiliumIoV1alpha1TracingPolicy**](CiliumIoV1alpha1Api.md#listCiliumIoV1alpha1TracingPolicy) | **GET** /apis/cilium.io/v1alpha1/tracingpolicies |  |
| [**listCiliumIoV1alpha1TracingPolicyNamespacedForAllNamespaces**](CiliumIoV1alpha1Api.md#listCiliumIoV1alpha1TracingPolicyNamespacedForAllNamespaces) | **GET** /apis/cilium.io/v1alpha1/tracingpoliciesnamespaced |  |
| [**patchCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**](CiliumIoV1alpha1Api.md#patchCiliumIoV1alpha1NamespacedTracingPolicyNamespaced) | **PATCH** /apis/cilium.io/v1alpha1/namespaces/{namespace}/tracingpoliciesnamespaced/{name} |  |
| [**patchCiliumIoV1alpha1TracingPolicy**](CiliumIoV1alpha1Api.md#patchCiliumIoV1alpha1TracingPolicy) | **PATCH** /apis/cilium.io/v1alpha1/tracingpolicies/{name} |  |
| [**readCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**](CiliumIoV1alpha1Api.md#readCiliumIoV1alpha1NamespacedTracingPolicyNamespaced) | **GET** /apis/cilium.io/v1alpha1/namespaces/{namespace}/tracingpoliciesnamespaced/{name} |  |
| [**readCiliumIoV1alpha1TracingPolicy**](CiliumIoV1alpha1Api.md#readCiliumIoV1alpha1TracingPolicy) | **GET** /apis/cilium.io/v1alpha1/tracingpolicies/{name} |  |
| [**replaceCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**](CiliumIoV1alpha1Api.md#replaceCiliumIoV1alpha1NamespacedTracingPolicyNamespaced) | **PUT** /apis/cilium.io/v1alpha1/namespaces/{namespace}/tracingpoliciesnamespaced/{name} |  |
| [**replaceCiliumIoV1alpha1TracingPolicy**](CiliumIoV1alpha1Api.md#replaceCiliumIoV1alpha1TracingPolicy) | **PUT** /apis/cilium.io/v1alpha1/tracingpolicies/{name} |  |


<a name="createCiliumIoV1alpha1NamespacedTracingPolicyNamespaced"></a>
# **createCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**
> io.cilium.v1alpha1.TracingPolicyNamespaced createCiliumIoV1alpha1NamespacedTracingPolicyNamespaced(namespace, pretty, dryRun, fieldManager, fieldValidation, io.cilium.v1alpha1.TracingPolicyNamespaced)



    create a TracingPolicyNamespaced

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **namespace** | **String**| object name and auth scope, such as for teams and projects | [default to null] |
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **dryRun** | **String**| When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed | [optional] [default to null] |
| **fieldManager** | **String**| fieldManager is a name associated with the actor or entity that is making these changes. The value must be less than or 128 characters long, and only contain printable characters, as defined by https://golang.org/pkg/unicode/#IsPrint. | [optional] [default to null] |
| **fieldValidation** | **String**| fieldValidation instructs the server on how to handle objects in the request (POST/PUT/PATCH) containing unknown or duplicate fields. Valid values are: - Ignore: This will ignore any unknown fields that are silently dropped from the object, and will ignore all but the last duplicate field that the decoder encounters. This is the default behavior prior to v1.23. - Warn: This will send a warning via the standard warning response header for each unknown field that is dropped from the object, and for each duplicate field that is encountered. The request will still succeed if there are no other errors, and will only persist the last of any duplicate fields. This is the default in v1.23+ - Strict: This will fail the request with a BadRequest error if any unknown fields would be dropped from the object, or if any duplicate fields are present. The error returned from the server will contain all unknown and duplicate fields encountered. | [optional] [default to null] |
| **io.cilium.v1alpha1.TracingPolicyNamespaced** | [**io.cilium.v1alpha1.TracingPolicyNamespaced**](../Models/io.cilium.v1alpha1.TracingPolicyNamespaced.md)|  | [optional] |

### Return type

[**io.cilium.v1alpha1.TracingPolicyNamespaced**](../Models/io.cilium.v1alpha1.TracingPolicyNamespaced.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/yaml
- **Accept**: application/json, application/yaml

<a name="createCiliumIoV1alpha1TracingPolicy"></a>
# **createCiliumIoV1alpha1TracingPolicy**
> io.cilium.v1alpha1.TracingPolicy createCiliumIoV1alpha1TracingPolicy(pretty, dryRun, fieldManager, fieldValidation, io.cilium.v1alpha1.TracingPolicy)



    create a TracingPolicy

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **dryRun** | **String**| When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed | [optional] [default to null] |
| **fieldManager** | **String**| fieldManager is a name associated with the actor or entity that is making these changes. The value must be less than or 128 characters long, and only contain printable characters, as defined by https://golang.org/pkg/unicode/#IsPrint. | [optional] [default to null] |
| **fieldValidation** | **String**| fieldValidation instructs the server on how to handle objects in the request (POST/PUT/PATCH) containing unknown or duplicate fields. Valid values are: - Ignore: This will ignore any unknown fields that are silently dropped from the object, and will ignore all but the last duplicate field that the decoder encounters. This is the default behavior prior to v1.23. - Warn: This will send a warning via the standard warning response header for each unknown field that is dropped from the object, and for each duplicate field that is encountered. The request will still succeed if there are no other errors, and will only persist the last of any duplicate fields. This is the default in v1.23+ - Strict: This will fail the request with a BadRequest error if any unknown fields would be dropped from the object, or if any duplicate fields are present. The error returned from the server will contain all unknown and duplicate fields encountered. | [optional] [default to null] |
| **io.cilium.v1alpha1.TracingPolicy** | [**io.cilium.v1alpha1.TracingPolicy**](../Models/io.cilium.v1alpha1.TracingPolicy.md)|  | [optional] |

### Return type

[**io.cilium.v1alpha1.TracingPolicy**](../Models/io.cilium.v1alpha1.TracingPolicy.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/yaml
- **Accept**: application/json, application/yaml

<a name="deleteCiliumIoV1alpha1CollectionNamespacedTracingPolicyNamespaced"></a>
# **deleteCiliumIoV1alpha1CollectionNamespacedTracingPolicyNamespaced**
> io.k8s.apimachinery.pkg.apis.meta.v1.Status deleteCiliumIoV1alpha1CollectionNamespacedTracingPolicyNamespaced(namespace, pretty, allowWatchBookmarks, continue, fieldSelector, labelSelector, limit, resourceVersion, resourceVersionMatch, sendInitialEvents, timeoutSeconds, watch)



    delete collection of TracingPolicyNamespaced

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **namespace** | **String**| object name and auth scope, such as for teams and projects | [default to null] |
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **allowWatchBookmarks** | **Boolean**| allowWatchBookmarks requests watch events with type \&quot;BOOKMARK\&quot;. Servers that do not implement bookmarks may ignore this flag and bookmarks are sent at the server&#39;s discretion. Clients should not assume bookmarks are returned at any specific interval, nor may they assume the server will send any BOOKMARK event during a session. If this is not a watch, this field is ignored. | [optional] [default to null] |
| **continue** | **String**| The continue option should be set when retrieving more results from the server. Since this value is server defined, clients may only use the continue value from a previous query result with identical query parameters (except for the value of continue) and the server may reject a continue value it does not recognize. If the specified continue value is no longer valid whether due to expiration (generally five to fifteen minutes) or a configuration change on the server, the server will respond with a 410 ResourceExpired error together with a continue token. If the client needs a consistent list, it must restart their list without the continue field. Otherwise, the client may send another list request with the token received with the 410 error, the server will respond with a list starting from the next key, but from the latest snapshot, which is inconsistent from the previous list results - objects that are created, modified, or deleted after the first list request will be included in the response, as long as their keys are after the \&quot;next key\&quot;.  This field is not supported when watch is true. Clients may start a watch from the last resourceVersion value returned by the server and not miss any modifications. | [optional] [default to null] |
| **fieldSelector** | **String**| A selector to restrict the list of returned objects by their fields. Defaults to everything. | [optional] [default to null] |
| **labelSelector** | **String**| A selector to restrict the list of returned objects by their labels. Defaults to everything. | [optional] [default to null] |
| **limit** | **Integer**| limit is a maximum number of responses to return for a list call. If more items exist, the server will set the &#x60;continue&#x60; field on the list metadata to a value that can be used with the same initial query to retrieve the next set of results. Setting a limit may return fewer than the requested amount of items (up to zero items) in the event all requested objects are filtered out and clients should only use the presence of the continue field to determine whether more results are available. Servers may choose not to support the limit argument and will return all of the available results. If limit is specified and the continue field is empty, clients may assume that no more results are available. This field is not supported if watch is true.  The server guarantees that the objects returned when using continue will be identical to issuing a single list call without a limit - that is, no objects created, modified, or deleted after the first request is issued will be included in any subsequent continued requests. This is sometimes referred to as a consistent snapshot, and ensures that a client that is using limit to receive smaller chunks of a very large result can ensure they see all possible objects. If objects are updated during a chunked list the version of the object that was present at the time the first list result was calculated is returned. | [optional] [default to null] |
| **resourceVersion** | **String**| resourceVersion sets a constraint on what resource versions a request may be served from. See https://kubernetes.io/docs/reference/using-api/api-concepts/#resource-versions for details.  Defaults to unset | [optional] [default to null] |
| **resourceVersionMatch** | **String**| resourceVersionMatch determines how resourceVersion is applied to list calls. It is highly recommended that resourceVersionMatch be set for list calls where resourceVersion is set See https://kubernetes.io/docs/reference/using-api/api-concepts/#resource-versions for details.  Defaults to unset | [optional] [default to null] |
| **sendInitialEvents** | **Boolean**| &#x60;sendInitialEvents&#x3D;true&#x60; may be set together with &#x60;watch&#x3D;true&#x60;. In that case, the watch stream will begin with synthetic events to produce the current state of objects in the collection. Once all such events have been sent, a synthetic \&quot;Bookmark\&quot; event  will be sent. The bookmark will report the ResourceVersion (RV) corresponding to the set of objects, and be marked with &#x60;\&quot;k8s.io/initial-events-end\&quot;: \&quot;true\&quot;&#x60; annotation. Afterwards, the watch stream will proceed as usual, sending watch events corresponding to changes (subsequent to the RV) to objects watched.  When &#x60;sendInitialEvents&#x60; option is set, we require &#x60;resourceVersionMatch&#x60; option to also be set. The semantic of the watch request is as following: - &#x60;resourceVersionMatch&#x60; &#x3D; NotOlderThan   is interpreted as \&quot;data at least as new as the provided &#x60;resourceVersion&#x60;\&quot;   and the bookmark event is send when the state is synced   to a &#x60;resourceVersion&#x60; at least as fresh as the one provided by the ListOptions.   If &#x60;resourceVersion&#x60; is unset, this is interpreted as \&quot;consistent read\&quot; and the   bookmark event is send when the state is synced at least to the moment   when request started being processed. - &#x60;resourceVersionMatch&#x60; set to any other value or unset   Invalid error is returned.  Defaults to true if &#x60;resourceVersion&#x3D;\&quot;\&quot;&#x60; or &#x60;resourceVersion&#x3D;\&quot;0\&quot;&#x60; (for backward compatibility reasons) and to false otherwise. | [optional] [default to null] |
| **timeoutSeconds** | **Integer**| Timeout for the list/watch call. This limits the duration of the call, regardless of any activity or inactivity. | [optional] [default to null] |
| **watch** | **Boolean**| Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. | [optional] [default to null] |

### Return type

[**io.k8s.apimachinery.pkg.apis.meta.v1.Status**](../Models/io.k8s.apimachinery.pkg.apis.meta.v1.Status.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/yaml

<a name="deleteCiliumIoV1alpha1CollectionTracingPolicy"></a>
# **deleteCiliumIoV1alpha1CollectionTracingPolicy**
> io.k8s.apimachinery.pkg.apis.meta.v1.Status deleteCiliumIoV1alpha1CollectionTracingPolicy(pretty, allowWatchBookmarks, continue, fieldSelector, labelSelector, limit, resourceVersion, resourceVersionMatch, sendInitialEvents, timeoutSeconds, watch)



    delete collection of TracingPolicy

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **allowWatchBookmarks** | **Boolean**| allowWatchBookmarks requests watch events with type \&quot;BOOKMARK\&quot;. Servers that do not implement bookmarks may ignore this flag and bookmarks are sent at the server&#39;s discretion. Clients should not assume bookmarks are returned at any specific interval, nor may they assume the server will send any BOOKMARK event during a session. If this is not a watch, this field is ignored. | [optional] [default to null] |
| **continue** | **String**| The continue option should be set when retrieving more results from the server. Since this value is server defined, clients may only use the continue value from a previous query result with identical query parameters (except for the value of continue) and the server may reject a continue value it does not recognize. If the specified continue value is no longer valid whether due to expiration (generally five to fifteen minutes) or a configuration change on the server, the server will respond with a 410 ResourceExpired error together with a continue token. If the client needs a consistent list, it must restart their list without the continue field. Otherwise, the client may send another list request with the token received with the 410 error, the server will respond with a list starting from the next key, but from the latest snapshot, which is inconsistent from the previous list results - objects that are created, modified, or deleted after the first list request will be included in the response, as long as their keys are after the \&quot;next key\&quot;.  This field is not supported when watch is true. Clients may start a watch from the last resourceVersion value returned by the server and not miss any modifications. | [optional] [default to null] |
| **fieldSelector** | **String**| A selector to restrict the list of returned objects by their fields. Defaults to everything. | [optional] [default to null] |
| **labelSelector** | **String**| A selector to restrict the list of returned objects by their labels. Defaults to everything. | [optional] [default to null] |
| **limit** | **Integer**| limit is a maximum number of responses to return for a list call. If more items exist, the server will set the &#x60;continue&#x60; field on the list metadata to a value that can be used with the same initial query to retrieve the next set of results. Setting a limit may return fewer than the requested amount of items (up to zero items) in the event all requested objects are filtered out and clients should only use the presence of the continue field to determine whether more results are available. Servers may choose not to support the limit argument and will return all of the available results. If limit is specified and the continue field is empty, clients may assume that no more results are available. This field is not supported if watch is true.  The server guarantees that the objects returned when using continue will be identical to issuing a single list call without a limit - that is, no objects created, modified, or deleted after the first request is issued will be included in any subsequent continued requests. This is sometimes referred to as a consistent snapshot, and ensures that a client that is using limit to receive smaller chunks of a very large result can ensure they see all possible objects. If objects are updated during a chunked list the version of the object that was present at the time the first list result was calculated is returned. | [optional] [default to null] |
| **resourceVersion** | **String**| resourceVersion sets a constraint on what resource versions a request may be served from. See https://kubernetes.io/docs/reference/using-api/api-concepts/#resource-versions for details.  Defaults to unset | [optional] [default to null] |
| **resourceVersionMatch** | **String**| resourceVersionMatch determines how resourceVersion is applied to list calls. It is highly recommended that resourceVersionMatch be set for list calls where resourceVersion is set See https://kubernetes.io/docs/reference/using-api/api-concepts/#resource-versions for details.  Defaults to unset | [optional] [default to null] |
| **sendInitialEvents** | **Boolean**| &#x60;sendInitialEvents&#x3D;true&#x60; may be set together with &#x60;watch&#x3D;true&#x60;. In that case, the watch stream will begin with synthetic events to produce the current state of objects in the collection. Once all such events have been sent, a synthetic \&quot;Bookmark\&quot; event  will be sent. The bookmark will report the ResourceVersion (RV) corresponding to the set of objects, and be marked with &#x60;\&quot;k8s.io/initial-events-end\&quot;: \&quot;true\&quot;&#x60; annotation. Afterwards, the watch stream will proceed as usual, sending watch events corresponding to changes (subsequent to the RV) to objects watched.  When &#x60;sendInitialEvents&#x60; option is set, we require &#x60;resourceVersionMatch&#x60; option to also be set. The semantic of the watch request is as following: - &#x60;resourceVersionMatch&#x60; &#x3D; NotOlderThan   is interpreted as \&quot;data at least as new as the provided &#x60;resourceVersion&#x60;\&quot;   and the bookmark event is send when the state is synced   to a &#x60;resourceVersion&#x60; at least as fresh as the one provided by the ListOptions.   If &#x60;resourceVersion&#x60; is unset, this is interpreted as \&quot;consistent read\&quot; and the   bookmark event is send when the state is synced at least to the moment   when request started being processed. - &#x60;resourceVersionMatch&#x60; set to any other value or unset   Invalid error is returned.  Defaults to true if &#x60;resourceVersion&#x3D;\&quot;\&quot;&#x60; or &#x60;resourceVersion&#x3D;\&quot;0\&quot;&#x60; (for backward compatibility reasons) and to false otherwise. | [optional] [default to null] |
| **timeoutSeconds** | **Integer**| Timeout for the list/watch call. This limits the duration of the call, regardless of any activity or inactivity. | [optional] [default to null] |
| **watch** | **Boolean**| Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. | [optional] [default to null] |

### Return type

[**io.k8s.apimachinery.pkg.apis.meta.v1.Status**](../Models/io.k8s.apimachinery.pkg.apis.meta.v1.Status.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/yaml

<a name="deleteCiliumIoV1alpha1NamespacedTracingPolicyNamespaced"></a>
# **deleteCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**
> io.k8s.apimachinery.pkg.apis.meta.v1.Status deleteCiliumIoV1alpha1NamespacedTracingPolicyNamespaced(name, namespace, pretty, dryRun, gracePeriodSeconds, orphanDependents, propagationPolicy, io.k8s.apimachinery.pkg.apis.meta.v1.DeleteOptions)



    delete a TracingPolicyNamespaced

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**| name of the TracingPolicyNamespaced | [default to null] |
| **namespace** | **String**| object name and auth scope, such as for teams and projects | [default to null] |
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **dryRun** | **String**| When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed | [optional] [default to null] |
| **gracePeriodSeconds** | **Integer**| The duration in seconds before the object should be deleted. Value must be non-negative integer. The value zero indicates delete immediately. If this value is nil, the default grace period for the specified type will be used. Defaults to a per object value if not specified. zero means delete immediately. | [optional] [default to null] |
| **orphanDependents** | **Boolean**| Deprecated: please use the PropagationPolicy, this field will be deprecated in 1.7. Should the dependent objects be orphaned. If true/false, the \&quot;orphan\&quot; finalizer will be added to/removed from the object&#39;s finalizers list. Either this field or PropagationPolicy may be set, but not both. | [optional] [default to null] |
| **propagationPolicy** | **String**| Whether and how garbage collection will be performed. Either this field or OrphanDependents may be set, but not both. The default policy is decided by the existing finalizer set in the metadata.finalizers and the resource-specific default policy. Acceptable values are: &#39;Orphan&#39; - orphan the dependents; &#39;Background&#39; - allow the garbage collector to delete the dependents in the background; &#39;Foreground&#39; - a cascading policy that deletes all dependents in the foreground. | [optional] [default to null] |
| **io.k8s.apimachinery.pkg.apis.meta.v1.DeleteOptions** | [**io.k8s.apimachinery.pkg.apis.meta.v1.DeleteOptions**](../Models/io.k8s.apimachinery.pkg.apis.meta.v1.DeleteOptions.md)|  | [optional] |

### Return type

[**io.k8s.apimachinery.pkg.apis.meta.v1.Status**](../Models/io.k8s.apimachinery.pkg.apis.meta.v1.Status.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/yaml
- **Accept**: application/json, application/yaml

<a name="deleteCiliumIoV1alpha1TracingPolicy"></a>
# **deleteCiliumIoV1alpha1TracingPolicy**
> io.k8s.apimachinery.pkg.apis.meta.v1.Status deleteCiliumIoV1alpha1TracingPolicy(name, pretty, dryRun, gracePeriodSeconds, orphanDependents, propagationPolicy, io.k8s.apimachinery.pkg.apis.meta.v1.DeleteOptions)



    delete a TracingPolicy

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**| name of the TracingPolicy | [default to null] |
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **dryRun** | **String**| When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed | [optional] [default to null] |
| **gracePeriodSeconds** | **Integer**| The duration in seconds before the object should be deleted. Value must be non-negative integer. The value zero indicates delete immediately. If this value is nil, the default grace period for the specified type will be used. Defaults to a per object value if not specified. zero means delete immediately. | [optional] [default to null] |
| **orphanDependents** | **Boolean**| Deprecated: please use the PropagationPolicy, this field will be deprecated in 1.7. Should the dependent objects be orphaned. If true/false, the \&quot;orphan\&quot; finalizer will be added to/removed from the object&#39;s finalizers list. Either this field or PropagationPolicy may be set, but not both. | [optional] [default to null] |
| **propagationPolicy** | **String**| Whether and how garbage collection will be performed. Either this field or OrphanDependents may be set, but not both. The default policy is decided by the existing finalizer set in the metadata.finalizers and the resource-specific default policy. Acceptable values are: &#39;Orphan&#39; - orphan the dependents; &#39;Background&#39; - allow the garbage collector to delete the dependents in the background; &#39;Foreground&#39; - a cascading policy that deletes all dependents in the foreground. | [optional] [default to null] |
| **io.k8s.apimachinery.pkg.apis.meta.v1.DeleteOptions** | [**io.k8s.apimachinery.pkg.apis.meta.v1.DeleteOptions**](../Models/io.k8s.apimachinery.pkg.apis.meta.v1.DeleteOptions.md)|  | [optional] |

### Return type

[**io.k8s.apimachinery.pkg.apis.meta.v1.Status**](../Models/io.k8s.apimachinery.pkg.apis.meta.v1.Status.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/yaml
- **Accept**: application/json, application/yaml

<a name="listCiliumIoV1alpha1NamespacedTracingPolicyNamespaced"></a>
# **listCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**
> io.cilium.v1alpha1.TracingPolicyNamespacedList listCiliumIoV1alpha1NamespacedTracingPolicyNamespaced(namespace, pretty, allowWatchBookmarks, continue, fieldSelector, labelSelector, limit, resourceVersion, resourceVersionMatch, sendInitialEvents, timeoutSeconds, watch)



    list objects of kind TracingPolicyNamespaced

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **namespace** | **String**| object name and auth scope, such as for teams and projects | [default to null] |
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **allowWatchBookmarks** | **Boolean**| allowWatchBookmarks requests watch events with type \&quot;BOOKMARK\&quot;. Servers that do not implement bookmarks may ignore this flag and bookmarks are sent at the server&#39;s discretion. Clients should not assume bookmarks are returned at any specific interval, nor may they assume the server will send any BOOKMARK event during a session. If this is not a watch, this field is ignored. | [optional] [default to null] |
| **continue** | **String**| The continue option should be set when retrieving more results from the server. Since this value is server defined, clients may only use the continue value from a previous query result with identical query parameters (except for the value of continue) and the server may reject a continue value it does not recognize. If the specified continue value is no longer valid whether due to expiration (generally five to fifteen minutes) or a configuration change on the server, the server will respond with a 410 ResourceExpired error together with a continue token. If the client needs a consistent list, it must restart their list without the continue field. Otherwise, the client may send another list request with the token received with the 410 error, the server will respond with a list starting from the next key, but from the latest snapshot, which is inconsistent from the previous list results - objects that are created, modified, or deleted after the first list request will be included in the response, as long as their keys are after the \&quot;next key\&quot;.  This field is not supported when watch is true. Clients may start a watch from the last resourceVersion value returned by the server and not miss any modifications. | [optional] [default to null] |
| **fieldSelector** | **String**| A selector to restrict the list of returned objects by their fields. Defaults to everything. | [optional] [default to null] |
| **labelSelector** | **String**| A selector to restrict the list of returned objects by their labels. Defaults to everything. | [optional] [default to null] |
| **limit** | **Integer**| limit is a maximum number of responses to return for a list call. If more items exist, the server will set the &#x60;continue&#x60; field on the list metadata to a value that can be used with the same initial query to retrieve the next set of results. Setting a limit may return fewer than the requested amount of items (up to zero items) in the event all requested objects are filtered out and clients should only use the presence of the continue field to determine whether more results are available. Servers may choose not to support the limit argument and will return all of the available results. If limit is specified and the continue field is empty, clients may assume that no more results are available. This field is not supported if watch is true.  The server guarantees that the objects returned when using continue will be identical to issuing a single list call without a limit - that is, no objects created, modified, or deleted after the first request is issued will be included in any subsequent continued requests. This is sometimes referred to as a consistent snapshot, and ensures that a client that is using limit to receive smaller chunks of a very large result can ensure they see all possible objects. If objects are updated during a chunked list the version of the object that was present at the time the first list result was calculated is returned. | [optional] [default to null] |
| **resourceVersion** | **String**| resourceVersion sets a constraint on what resource versions a request may be served from. See https://kubernetes.io/docs/reference/using-api/api-concepts/#resource-versions for details.  Defaults to unset | [optional] [default to null] |
| **resourceVersionMatch** | **String**| resourceVersionMatch determines how resourceVersion is applied to list calls. It is highly recommended that resourceVersionMatch be set for list calls where resourceVersion is set See https://kubernetes.io/docs/reference/using-api/api-concepts/#resource-versions for details.  Defaults to unset | [optional] [default to null] |
| **sendInitialEvents** | **Boolean**| &#x60;sendInitialEvents&#x3D;true&#x60; may be set together with &#x60;watch&#x3D;true&#x60;. In that case, the watch stream will begin with synthetic events to produce the current state of objects in the collection. Once all such events have been sent, a synthetic \&quot;Bookmark\&quot; event  will be sent. The bookmark will report the ResourceVersion (RV) corresponding to the set of objects, and be marked with &#x60;\&quot;k8s.io/initial-events-end\&quot;: \&quot;true\&quot;&#x60; annotation. Afterwards, the watch stream will proceed as usual, sending watch events corresponding to changes (subsequent to the RV) to objects watched.  When &#x60;sendInitialEvents&#x60; option is set, we require &#x60;resourceVersionMatch&#x60; option to also be set. The semantic of the watch request is as following: - &#x60;resourceVersionMatch&#x60; &#x3D; NotOlderThan   is interpreted as \&quot;data at least as new as the provided &#x60;resourceVersion&#x60;\&quot;   and the bookmark event is send when the state is synced   to a &#x60;resourceVersion&#x60; at least as fresh as the one provided by the ListOptions.   If &#x60;resourceVersion&#x60; is unset, this is interpreted as \&quot;consistent read\&quot; and the   bookmark event is send when the state is synced at least to the moment   when request started being processed. - &#x60;resourceVersionMatch&#x60; set to any other value or unset   Invalid error is returned.  Defaults to true if &#x60;resourceVersion&#x3D;\&quot;\&quot;&#x60; or &#x60;resourceVersion&#x3D;\&quot;0\&quot;&#x60; (for backward compatibility reasons) and to false otherwise. | [optional] [default to null] |
| **timeoutSeconds** | **Integer**| Timeout for the list/watch call. This limits the duration of the call, regardless of any activity or inactivity. | [optional] [default to null] |
| **watch** | **Boolean**| Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. | [optional] [default to null] |

### Return type

[**io.cilium.v1alpha1.TracingPolicyNamespacedList**](../Models/io.cilium.v1alpha1.TracingPolicyNamespacedList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/yaml

<a name="listCiliumIoV1alpha1TracingPolicy"></a>
# **listCiliumIoV1alpha1TracingPolicy**
> io.cilium.v1alpha1.TracingPolicyList listCiliumIoV1alpha1TracingPolicy(pretty, allowWatchBookmarks, continue, fieldSelector, labelSelector, limit, resourceVersion, resourceVersionMatch, sendInitialEvents, timeoutSeconds, watch)



    list objects of kind TracingPolicy

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **allowWatchBookmarks** | **Boolean**| allowWatchBookmarks requests watch events with type \&quot;BOOKMARK\&quot;. Servers that do not implement bookmarks may ignore this flag and bookmarks are sent at the server&#39;s discretion. Clients should not assume bookmarks are returned at any specific interval, nor may they assume the server will send any BOOKMARK event during a session. If this is not a watch, this field is ignored. | [optional] [default to null] |
| **continue** | **String**| The continue option should be set when retrieving more results from the server. Since this value is server defined, clients may only use the continue value from a previous query result with identical query parameters (except for the value of continue) and the server may reject a continue value it does not recognize. If the specified continue value is no longer valid whether due to expiration (generally five to fifteen minutes) or a configuration change on the server, the server will respond with a 410 ResourceExpired error together with a continue token. If the client needs a consistent list, it must restart their list without the continue field. Otherwise, the client may send another list request with the token received with the 410 error, the server will respond with a list starting from the next key, but from the latest snapshot, which is inconsistent from the previous list results - objects that are created, modified, or deleted after the first list request will be included in the response, as long as their keys are after the \&quot;next key\&quot;.  This field is not supported when watch is true. Clients may start a watch from the last resourceVersion value returned by the server and not miss any modifications. | [optional] [default to null] |
| **fieldSelector** | **String**| A selector to restrict the list of returned objects by their fields. Defaults to everything. | [optional] [default to null] |
| **labelSelector** | **String**| A selector to restrict the list of returned objects by their labels. Defaults to everything. | [optional] [default to null] |
| **limit** | **Integer**| limit is a maximum number of responses to return for a list call. If more items exist, the server will set the &#x60;continue&#x60; field on the list metadata to a value that can be used with the same initial query to retrieve the next set of results. Setting a limit may return fewer than the requested amount of items (up to zero items) in the event all requested objects are filtered out and clients should only use the presence of the continue field to determine whether more results are available. Servers may choose not to support the limit argument and will return all of the available results. If limit is specified and the continue field is empty, clients may assume that no more results are available. This field is not supported if watch is true.  The server guarantees that the objects returned when using continue will be identical to issuing a single list call without a limit - that is, no objects created, modified, or deleted after the first request is issued will be included in any subsequent continued requests. This is sometimes referred to as a consistent snapshot, and ensures that a client that is using limit to receive smaller chunks of a very large result can ensure they see all possible objects. If objects are updated during a chunked list the version of the object that was present at the time the first list result was calculated is returned. | [optional] [default to null] |
| **resourceVersion** | **String**| resourceVersion sets a constraint on what resource versions a request may be served from. See https://kubernetes.io/docs/reference/using-api/api-concepts/#resource-versions for details.  Defaults to unset | [optional] [default to null] |
| **resourceVersionMatch** | **String**| resourceVersionMatch determines how resourceVersion is applied to list calls. It is highly recommended that resourceVersionMatch be set for list calls where resourceVersion is set See https://kubernetes.io/docs/reference/using-api/api-concepts/#resource-versions for details.  Defaults to unset | [optional] [default to null] |
| **sendInitialEvents** | **Boolean**| &#x60;sendInitialEvents&#x3D;true&#x60; may be set together with &#x60;watch&#x3D;true&#x60;. In that case, the watch stream will begin with synthetic events to produce the current state of objects in the collection. Once all such events have been sent, a synthetic \&quot;Bookmark\&quot; event  will be sent. The bookmark will report the ResourceVersion (RV) corresponding to the set of objects, and be marked with &#x60;\&quot;k8s.io/initial-events-end\&quot;: \&quot;true\&quot;&#x60; annotation. Afterwards, the watch stream will proceed as usual, sending watch events corresponding to changes (subsequent to the RV) to objects watched.  When &#x60;sendInitialEvents&#x60; option is set, we require &#x60;resourceVersionMatch&#x60; option to also be set. The semantic of the watch request is as following: - &#x60;resourceVersionMatch&#x60; &#x3D; NotOlderThan   is interpreted as \&quot;data at least as new as the provided &#x60;resourceVersion&#x60;\&quot;   and the bookmark event is send when the state is synced   to a &#x60;resourceVersion&#x60; at least as fresh as the one provided by the ListOptions.   If &#x60;resourceVersion&#x60; is unset, this is interpreted as \&quot;consistent read\&quot; and the   bookmark event is send when the state is synced at least to the moment   when request started being processed. - &#x60;resourceVersionMatch&#x60; set to any other value or unset   Invalid error is returned.  Defaults to true if &#x60;resourceVersion&#x3D;\&quot;\&quot;&#x60; or &#x60;resourceVersion&#x3D;\&quot;0\&quot;&#x60; (for backward compatibility reasons) and to false otherwise. | [optional] [default to null] |
| **timeoutSeconds** | **Integer**| Timeout for the list/watch call. This limits the duration of the call, regardless of any activity or inactivity. | [optional] [default to null] |
| **watch** | **Boolean**| Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. | [optional] [default to null] |

### Return type

[**io.cilium.v1alpha1.TracingPolicyList**](../Models/io.cilium.v1alpha1.TracingPolicyList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/yaml

<a name="listCiliumIoV1alpha1TracingPolicyNamespacedForAllNamespaces"></a>
# **listCiliumIoV1alpha1TracingPolicyNamespacedForAllNamespaces**
> io.cilium.v1alpha1.TracingPolicyNamespacedList listCiliumIoV1alpha1TracingPolicyNamespacedForAllNamespaces(allowWatchBookmarks, continue, fieldSelector, labelSelector, limit, pretty, resourceVersion, resourceVersionMatch, sendInitialEvents, timeoutSeconds, watch)



    list objects of kind TracingPolicyNamespaced

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **allowWatchBookmarks** | **Boolean**| allowWatchBookmarks requests watch events with type \&quot;BOOKMARK\&quot;. Servers that do not implement bookmarks may ignore this flag and bookmarks are sent at the server&#39;s discretion. Clients should not assume bookmarks are returned at any specific interval, nor may they assume the server will send any BOOKMARK event during a session. If this is not a watch, this field is ignored. | [optional] [default to null] |
| **continue** | **String**| The continue option should be set when retrieving more results from the server. Since this value is server defined, clients may only use the continue value from a previous query result with identical query parameters (except for the value of continue) and the server may reject a continue value it does not recognize. If the specified continue value is no longer valid whether due to expiration (generally five to fifteen minutes) or a configuration change on the server, the server will respond with a 410 ResourceExpired error together with a continue token. If the client needs a consistent list, it must restart their list without the continue field. Otherwise, the client may send another list request with the token received with the 410 error, the server will respond with a list starting from the next key, but from the latest snapshot, which is inconsistent from the previous list results - objects that are created, modified, or deleted after the first list request will be included in the response, as long as their keys are after the \&quot;next key\&quot;.  This field is not supported when watch is true. Clients may start a watch from the last resourceVersion value returned by the server and not miss any modifications. | [optional] [default to null] |
| **fieldSelector** | **String**| A selector to restrict the list of returned objects by their fields. Defaults to everything. | [optional] [default to null] |
| **labelSelector** | **String**| A selector to restrict the list of returned objects by their labels. Defaults to everything. | [optional] [default to null] |
| **limit** | **Integer**| limit is a maximum number of responses to return for a list call. If more items exist, the server will set the &#x60;continue&#x60; field on the list metadata to a value that can be used with the same initial query to retrieve the next set of results. Setting a limit may return fewer than the requested amount of items (up to zero items) in the event all requested objects are filtered out and clients should only use the presence of the continue field to determine whether more results are available. Servers may choose not to support the limit argument and will return all of the available results. If limit is specified and the continue field is empty, clients may assume that no more results are available. This field is not supported if watch is true.  The server guarantees that the objects returned when using continue will be identical to issuing a single list call without a limit - that is, no objects created, modified, or deleted after the first request is issued will be included in any subsequent continued requests. This is sometimes referred to as a consistent snapshot, and ensures that a client that is using limit to receive smaller chunks of a very large result can ensure they see all possible objects. If objects are updated during a chunked list the version of the object that was present at the time the first list result was calculated is returned. | [optional] [default to null] |
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **resourceVersion** | **String**| resourceVersion sets a constraint on what resource versions a request may be served from. See https://kubernetes.io/docs/reference/using-api/api-concepts/#resource-versions for details.  Defaults to unset | [optional] [default to null] |
| **resourceVersionMatch** | **String**| resourceVersionMatch determines how resourceVersion is applied to list calls. It is highly recommended that resourceVersionMatch be set for list calls where resourceVersion is set See https://kubernetes.io/docs/reference/using-api/api-concepts/#resource-versions for details.  Defaults to unset | [optional] [default to null] |
| **sendInitialEvents** | **Boolean**| &#x60;sendInitialEvents&#x3D;true&#x60; may be set together with &#x60;watch&#x3D;true&#x60;. In that case, the watch stream will begin with synthetic events to produce the current state of objects in the collection. Once all such events have been sent, a synthetic \&quot;Bookmark\&quot; event  will be sent. The bookmark will report the ResourceVersion (RV) corresponding to the set of objects, and be marked with &#x60;\&quot;k8s.io/initial-events-end\&quot;: \&quot;true\&quot;&#x60; annotation. Afterwards, the watch stream will proceed as usual, sending watch events corresponding to changes (subsequent to the RV) to objects watched.  When &#x60;sendInitialEvents&#x60; option is set, we require &#x60;resourceVersionMatch&#x60; option to also be set. The semantic of the watch request is as following: - &#x60;resourceVersionMatch&#x60; &#x3D; NotOlderThan   is interpreted as \&quot;data at least as new as the provided &#x60;resourceVersion&#x60;\&quot;   and the bookmark event is send when the state is synced   to a &#x60;resourceVersion&#x60; at least as fresh as the one provided by the ListOptions.   If &#x60;resourceVersion&#x60; is unset, this is interpreted as \&quot;consistent read\&quot; and the   bookmark event is send when the state is synced at least to the moment   when request started being processed. - &#x60;resourceVersionMatch&#x60; set to any other value or unset   Invalid error is returned.  Defaults to true if &#x60;resourceVersion&#x3D;\&quot;\&quot;&#x60; or &#x60;resourceVersion&#x3D;\&quot;0\&quot;&#x60; (for backward compatibility reasons) and to false otherwise. | [optional] [default to null] |
| **timeoutSeconds** | **Integer**| Timeout for the list/watch call. This limits the duration of the call, regardless of any activity or inactivity. | [optional] [default to null] |
| **watch** | **Boolean**| Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. | [optional] [default to null] |

### Return type

[**io.cilium.v1alpha1.TracingPolicyNamespacedList**](../Models/io.cilium.v1alpha1.TracingPolicyNamespacedList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/yaml

<a name="patchCiliumIoV1alpha1NamespacedTracingPolicyNamespaced"></a>
# **patchCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**
> io.cilium.v1alpha1.TracingPolicyNamespaced patchCiliumIoV1alpha1NamespacedTracingPolicyNamespaced(name, namespace, pretty, dryRun, fieldManager, fieldValidation, force, body)



    partially update the specified TracingPolicyNamespaced

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**| name of the TracingPolicyNamespaced | [default to null] |
| **namespace** | **String**| object name and auth scope, such as for teams and projects | [default to null] |
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **dryRun** | **String**| When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed | [optional] [default to null] |
| **fieldManager** | **String**| fieldManager is a name associated with the actor or entity that is making these changes. The value must be less than or 128 characters long, and only contain printable characters, as defined by https://golang.org/pkg/unicode/#IsPrint. This field is required for apply requests (application/apply-patch) but optional for non-apply patch types (JsonPatch, MergePatch, StrategicMergePatch). | [optional] [default to null] |
| **fieldValidation** | **String**| fieldValidation instructs the server on how to handle objects in the request (POST/PUT/PATCH) containing unknown or duplicate fields. Valid values are: - Ignore: This will ignore any unknown fields that are silently dropped from the object, and will ignore all but the last duplicate field that the decoder encounters. This is the default behavior prior to v1.23. - Warn: This will send a warning via the standard warning response header for each unknown field that is dropped from the object, and for each duplicate field that is encountered. The request will still succeed if there are no other errors, and will only persist the last of any duplicate fields. This is the default in v1.23+ - Strict: This will fail the request with a BadRequest error if any unknown fields would be dropped from the object, or if any duplicate fields are present. The error returned from the server will contain all unknown and duplicate fields encountered. | [optional] [default to null] |
| **force** | **Boolean**| Force is going to \&quot;force\&quot; Apply requests. It means user will re-acquire conflicting fields owned by other people. Force flag must be unset for non-apply patch requests. | [optional] [default to null] |
| **body** | **Object**|  | [optional] |

### Return type

[**io.cilium.v1alpha1.TracingPolicyNamespaced**](../Models/io.cilium.v1alpha1.TracingPolicyNamespaced.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/apply-patch+yaml, application/json-patch+json, application/merge-patch+json
- **Accept**: application/json, application/yaml

<a name="patchCiliumIoV1alpha1TracingPolicy"></a>
# **patchCiliumIoV1alpha1TracingPolicy**
> io.cilium.v1alpha1.TracingPolicy patchCiliumIoV1alpha1TracingPolicy(name, pretty, dryRun, fieldManager, fieldValidation, force, body)



    partially update the specified TracingPolicy

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**| name of the TracingPolicy | [default to null] |
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **dryRun** | **String**| When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed | [optional] [default to null] |
| **fieldManager** | **String**| fieldManager is a name associated with the actor or entity that is making these changes. The value must be less than or 128 characters long, and only contain printable characters, as defined by https://golang.org/pkg/unicode/#IsPrint. This field is required for apply requests (application/apply-patch) but optional for non-apply patch types (JsonPatch, MergePatch, StrategicMergePatch). | [optional] [default to null] |
| **fieldValidation** | **String**| fieldValidation instructs the server on how to handle objects in the request (POST/PUT/PATCH) containing unknown or duplicate fields. Valid values are: - Ignore: This will ignore any unknown fields that are silently dropped from the object, and will ignore all but the last duplicate field that the decoder encounters. This is the default behavior prior to v1.23. - Warn: This will send a warning via the standard warning response header for each unknown field that is dropped from the object, and for each duplicate field that is encountered. The request will still succeed if there are no other errors, and will only persist the last of any duplicate fields. This is the default in v1.23+ - Strict: This will fail the request with a BadRequest error if any unknown fields would be dropped from the object, or if any duplicate fields are present. The error returned from the server will contain all unknown and duplicate fields encountered. | [optional] [default to null] |
| **force** | **Boolean**| Force is going to \&quot;force\&quot; Apply requests. It means user will re-acquire conflicting fields owned by other people. Force flag must be unset for non-apply patch requests. | [optional] [default to null] |
| **body** | **Object**|  | [optional] |

### Return type

[**io.cilium.v1alpha1.TracingPolicy**](../Models/io.cilium.v1alpha1.TracingPolicy.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/apply-patch+yaml, application/json-patch+json, application/merge-patch+json
- **Accept**: application/json, application/yaml

<a name="readCiliumIoV1alpha1NamespacedTracingPolicyNamespaced"></a>
# **readCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**
> io.cilium.v1alpha1.TracingPolicyNamespaced readCiliumIoV1alpha1NamespacedTracingPolicyNamespaced(name, namespace, pretty, resourceVersion)



    read the specified TracingPolicyNamespaced

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**| name of the TracingPolicyNamespaced | [default to null] |
| **namespace** | **String**| object name and auth scope, such as for teams and projects | [default to null] |
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **resourceVersion** | **String**| resourceVersion sets a constraint on what resource versions a request may be served from. See https://kubernetes.io/docs/reference/using-api/api-concepts/#resource-versions for details.  Defaults to unset | [optional] [default to null] |

### Return type

[**io.cilium.v1alpha1.TracingPolicyNamespaced**](../Models/io.cilium.v1alpha1.TracingPolicyNamespaced.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/yaml

<a name="readCiliumIoV1alpha1TracingPolicy"></a>
# **readCiliumIoV1alpha1TracingPolicy**
> io.cilium.v1alpha1.TracingPolicy readCiliumIoV1alpha1TracingPolicy(name, pretty, resourceVersion)



    read the specified TracingPolicy

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**| name of the TracingPolicy | [default to null] |
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **resourceVersion** | **String**| resourceVersion sets a constraint on what resource versions a request may be served from. See https://kubernetes.io/docs/reference/using-api/api-concepts/#resource-versions for details.  Defaults to unset | [optional] [default to null] |

### Return type

[**io.cilium.v1alpha1.TracingPolicy**](../Models/io.cilium.v1alpha1.TracingPolicy.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/yaml

<a name="replaceCiliumIoV1alpha1NamespacedTracingPolicyNamespaced"></a>
# **replaceCiliumIoV1alpha1NamespacedTracingPolicyNamespaced**
> io.cilium.v1alpha1.TracingPolicyNamespaced replaceCiliumIoV1alpha1NamespacedTracingPolicyNamespaced(name, namespace, pretty, dryRun, fieldManager, fieldValidation, io.cilium.v1alpha1.TracingPolicyNamespaced)



    replace the specified TracingPolicyNamespaced

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**| name of the TracingPolicyNamespaced | [default to null] |
| **namespace** | **String**| object name and auth scope, such as for teams and projects | [default to null] |
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **dryRun** | **String**| When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed | [optional] [default to null] |
| **fieldManager** | **String**| fieldManager is a name associated with the actor or entity that is making these changes. The value must be less than or 128 characters long, and only contain printable characters, as defined by https://golang.org/pkg/unicode/#IsPrint. | [optional] [default to null] |
| **fieldValidation** | **String**| fieldValidation instructs the server on how to handle objects in the request (POST/PUT/PATCH) containing unknown or duplicate fields. Valid values are: - Ignore: This will ignore any unknown fields that are silently dropped from the object, and will ignore all but the last duplicate field that the decoder encounters. This is the default behavior prior to v1.23. - Warn: This will send a warning via the standard warning response header for each unknown field that is dropped from the object, and for each duplicate field that is encountered. The request will still succeed if there are no other errors, and will only persist the last of any duplicate fields. This is the default in v1.23+ - Strict: This will fail the request with a BadRequest error if any unknown fields would be dropped from the object, or if any duplicate fields are present. The error returned from the server will contain all unknown and duplicate fields encountered. | [optional] [default to null] |
| **io.cilium.v1alpha1.TracingPolicyNamespaced** | [**io.cilium.v1alpha1.TracingPolicyNamespaced**](../Models/io.cilium.v1alpha1.TracingPolicyNamespaced.md)|  | [optional] |

### Return type

[**io.cilium.v1alpha1.TracingPolicyNamespaced**](../Models/io.cilium.v1alpha1.TracingPolicyNamespaced.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/yaml
- **Accept**: application/json, application/yaml

<a name="replaceCiliumIoV1alpha1TracingPolicy"></a>
# **replaceCiliumIoV1alpha1TracingPolicy**
> io.cilium.v1alpha1.TracingPolicy replaceCiliumIoV1alpha1TracingPolicy(name, pretty, dryRun, fieldManager, fieldValidation, io.cilium.v1alpha1.TracingPolicy)



    replace the specified TracingPolicy

### Parameters

|Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **name** | **String**| name of the TracingPolicy | [default to null] |
| **pretty** | **String**| If &#39;true&#39;, then the output is pretty printed. | [optional] [default to null] |
| **dryRun** | **String**| When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed | [optional] [default to null] |
| **fieldManager** | **String**| fieldManager is a name associated with the actor or entity that is making these changes. The value must be less than or 128 characters long, and only contain printable characters, as defined by https://golang.org/pkg/unicode/#IsPrint. | [optional] [default to null] |
| **fieldValidation** | **String**| fieldValidation instructs the server on how to handle objects in the request (POST/PUT/PATCH) containing unknown or duplicate fields. Valid values are: - Ignore: This will ignore any unknown fields that are silently dropped from the object, and will ignore all but the last duplicate field that the decoder encounters. This is the default behavior prior to v1.23. - Warn: This will send a warning via the standard warning response header for each unknown field that is dropped from the object, and for each duplicate field that is encountered. The request will still succeed if there are no other errors, and will only persist the last of any duplicate fields. This is the default in v1.23+ - Strict: This will fail the request with a BadRequest error if any unknown fields would be dropped from the object, or if any duplicate fields are present. The error returned from the server will contain all unknown and duplicate fields encountered. | [optional] [default to null] |
| **io.cilium.v1alpha1.TracingPolicy** | [**io.cilium.v1alpha1.TracingPolicy**](../Models/io.cilium.v1alpha1.TracingPolicy.md)|  | [optional] |

### Return type

[**io.cilium.v1alpha1.TracingPolicy**](../Models/io.cilium.v1alpha1.TracingPolicy.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json, application/yaml
- **Accept**: application/json, application/yaml

