# V1alpha1PullRequestGeneratorAzureDevOps

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api** | Option<**String**> | The Azure DevOps API URL to talk to. If blank, use https://dev.azure.com/. | [optional]
**labels** | Option<**Vec<String>**> |  | [optional]
**organization** | Option<**String**> | Azure DevOps org to scan. Required. | [optional]
**project** | Option<**String**> | Azure DevOps project name to scan. Required. | [optional]
**repo** | Option<**String**> | Azure DevOps repo name to scan. Required. | [optional]
**token_ref** | Option<[**models::V1alpha1SecretRef**](v1alpha1SecretRef.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


