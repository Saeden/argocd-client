# V1alpha1PullRequestGeneratorBitbucketServer

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api** | Option<**String**> | The Bitbucket REST API URL to talk to e.g. https://bitbucket.org/rest Required. | [optional]
**basic_auth** | Option<[**models::V1alpha1BasicAuthBitbucketServer**](v1alpha1BasicAuthBitbucketServer.md)> |  | [optional]
**bearer_token** | Option<[**models::V1alpha1BearerTokenBitbucket**](v1alpha1BearerTokenBitbucket.md)> |  | [optional]
**ca_ref** | Option<[**models::V1alpha1ConfigMapKeyRef**](v1alpha1ConfigMapKeyRef.md)> |  | [optional]
**insecure** | Option<**bool**> |  | [optional]
**project** | Option<**String**> | Project to scan. Required. | [optional]
**repo** | Option<**String**> | Repo name to scan. Required. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


