# V1alpha1ScmProviderGeneratorGitlab

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**all_branches** | Option<**bool**> | Scan all branches instead of just the default branch. | [optional]
**api** | Option<**String**> | The Gitlab API URL to talk to. | [optional]
**ca_ref** | Option<[**models::V1alpha1ConfigMapKeyRef**](v1alpha1ConfigMapKeyRef.md)> |  | [optional]
**group** | Option<**String**> | Gitlab group to scan. Required.  You can use either the project id (recommended) or the full namespaced path. | [optional]
**include_shared_projects** | Option<**bool**> |  | [optional]
**include_subgroups** | Option<**bool**> |  | [optional]
**insecure** | Option<**bool**> |  | [optional]
**token_ref** | Option<[**models::V1alpha1SecretRef**](v1alpha1SecretRef.md)> |  | [optional]
**topic** | Option<**String**> | Filter repos list based on Gitlab Topic. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


