# V1alpha1ScmProviderGeneratorAwsCodeCommit

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**all_branches** | Option<**bool**> | Scan all branches instead of just the default branch. | [optional]
**region** | Option<**String**> | Region provides the AWS region to discover repos. if not provided, AppSet controller will infer the current region from environment. | [optional]
**role** | Option<**String**> | Role provides the AWS IAM role to assume, for cross-account repo discovery if not provided, AppSet controller will use its pod/node identity to discover. | [optional]
**tag_filters** | Option<[**Vec<models::V1alpha1TagFilter>**](v1alpha1TagFilter.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


