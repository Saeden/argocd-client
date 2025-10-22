# V1alpha1PullRequestGeneratorBitbucket

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api** | Option<**String**> | The Bitbucket REST API URL to talk to. If blank, uses https://api.bitbucket.org/2.0. | [optional]
**basic_auth** | Option<[**models::V1alpha1BasicAuthBitbucketServer**](v1alpha1BasicAuthBitbucketServer.md)> |  | [optional]
**bearer_token** | Option<[**models::V1alpha1BearerTokenBitbucketCloud**](v1alpha1BearerTokenBitbucketCloud.md)> |  | [optional]
**owner** | Option<**String**> | Workspace to scan. Required. | [optional]
**repo** | Option<**String**> | Repo name to scan. Required. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


