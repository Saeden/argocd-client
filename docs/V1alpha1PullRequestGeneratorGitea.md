# V1alpha1PullRequestGeneratorGitea

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api** | Option<**String**> |  | [optional]
**insecure** | Option<**bool**> | Allow insecure tls, for self-signed certificates; default: false. | [optional]
**labels** | Option<**Vec<String>**> |  | [optional]
**owner** | Option<**String**> | Gitea org or user to scan. Required. | [optional]
**repo** | Option<**String**> | Gitea repo name to scan. Required. | [optional]
**token_ref** | Option<[**models::V1alpha1SecretRef**](v1alpha1SecretRef.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


