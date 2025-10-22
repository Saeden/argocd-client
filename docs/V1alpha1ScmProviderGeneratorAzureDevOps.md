# V1alpha1ScmProviderGeneratorAzureDevOps

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**access_token_ref** | Option<[**models::V1alpha1SecretRef**](v1alpha1SecretRef.md)> |  | [optional]
**all_branches** | Option<**bool**> | Scan all branches instead of just the default branch. | [optional]
**api** | Option<**String**> | The URL to Azure DevOps. If blank, use https://dev.azure.com. | [optional]
**organization** | Option<**String**> | Azure Devops organization. Required. E.g. \"my-organization\". | [optional]
**team_project** | Option<**String**> | Azure Devops team project. Required. E.g. \"my-team\". | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


