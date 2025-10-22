# V1alpha1ScmProviderGeneratorBitbucketServer

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**all_branches** | Option<**bool**> | Scan all branches instead of just the default branch. | [optional]
**api** | Option<**String**> | The Bitbucket Server REST API URL to talk to. Required. | [optional]
**basic_auth** | Option<[**models::V1alpha1BasicAuthBitbucketServer**](v1alpha1BasicAuthBitbucketServer.md)> |  | [optional]
**bearer_token** | Option<[**models::V1alpha1BearerTokenBitbucket**](v1alpha1BearerTokenBitbucket.md)> |  | [optional]
**ca_ref** | Option<[**models::V1alpha1ConfigMapKeyRef**](v1alpha1ConfigMapKeyRef.md)> |  | [optional]
**insecure** | Option<**bool**> |  | [optional]
**project** | Option<**String**> | Project to scan. Required. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


