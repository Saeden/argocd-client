# V1alpha1ScmProviderGeneratorGithub

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**all_branches** | Option<**bool**> | Scan all branches instead of just the default branch. | [optional]
**api** | Option<**String**> | The GitHub API URL to talk to. If blank, use https://api.github.com/. | [optional]
**app_secret_name** | Option<**String**> | AppSecretName is a reference to a GitHub App repo-creds secret. | [optional]
**organization** | Option<**String**> | GitHub org to scan. Required. | [optional]
**token_ref** | Option<[**models::V1alpha1SecretRef**](v1alpha1SecretRef.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


