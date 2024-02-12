# io_cilium_v1alpha1_TracingPolicy_spec_kprobes_inner_selectors_inner_matchActions_inner
## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
| **action** | **String** | Action to execute. | [default to null] |
| **argError** | **Integer** | error value for override action | [optional] [default to null] |
| **argFd** | **Integer** | An arg index for the fd for fdInstall action | [optional] [default to null] |
| **argFqdn** | **String** | A FQDN to lookup for the dnsLookup action | [optional] [default to null] |
| **argName** | **Integer** | An arg index for the filename for fdInstall action | [optional] [default to null] |
| **argSig** | **Integer** | A signal number for signal action | [optional] [default to null] |
| **argSock** | **Integer** | An arg index for the sock for trackSock and untrackSock actions | [optional] [default to null] |
| **argUrl** | **String** | A URL for the getUrl action | [optional] [default to null] |
| **rateLimit** | **String** | A time period within which repeated messages will not be posted. Can be specified in seconds (default or with &#39;s&#39; suffix), minutes (&#39;m&#39; suffix) or hours (&#39;h&#39; suffix). Only valid with the post action. | [optional] [default to null] |
| **stackTrace** | **Boolean** | Enable stack trace export. Only valid with the post action. | [optional] [default to null] |

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

