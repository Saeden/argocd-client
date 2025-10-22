# V1alpha1PullRequestGeneratorGithub

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api** | Option<**String**> | The GitHub API URL to talk to. If blank, use https://api.github.com/. | [optional]
**app_secret_name** | Option<**String**> | AppSecretName is a reference to a GitHub App repo-creds secret with permission to access pull requests. | [optional]
**labels** | Option<**Vec<String>**> |  | [optional]
**owner** | Option<**String**> | GitHub org or user to scan. Required. | [optional]
**repo** | Option<**String**> | GitHub repo name to scan. Required. | [optional]
**token_ref** | Option<[**models::V1alpha1SecretRef**](v1alpha1SecretRef.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


