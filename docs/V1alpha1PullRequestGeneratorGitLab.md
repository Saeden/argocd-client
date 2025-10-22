# V1alpha1PullRequestGeneratorGitLab

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api** | Option<**String**> | The GitLab API URL to talk to. If blank, uses https://gitlab.com/. | [optional]
**ca_ref** | Option<[**models::V1alpha1ConfigMapKeyRef**](v1alpha1ConfigMapKeyRef.md)> |  | [optional]
**insecure** | Option<**bool**> |  | [optional]
**labels** | Option<**Vec<String>**> |  | [optional]
**project** | Option<**String**> | GitLab project to scan. Required. | [optional]
**pull_request_state** | Option<**String**> | PullRequestState is an additional MRs filter to get only those with a certain state. Default: \"\" (all states). Valid values: opened, closed, merged, locked\". | [optional]
**token_ref** | Option<[**models::V1alpha1SecretRef**](v1alpha1SecretRef.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


