# V1alpha1ApplicationSetSpec

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**apply_nested_selectors** | Option<**bool**> | ApplyNestedSelectors enables selectors defined within the generators of two level-nested matrix or merge generators Deprecated: This field is ignored, and the behavior is always enabled. The field will be removed in a future version of the ApplicationSet CRD. | [optional]
**generators** | Option<[**Vec<models::V1alpha1ApplicationSetGenerator>**](v1alpha1ApplicationSetGenerator.md)> |  | [optional]
**go_template** | Option<**bool**> |  | [optional]
**go_template_options** | Option<**Vec<String>**> |  | [optional]
**ignore_application_differences** | Option<[**Vec<models::V1alpha1ApplicationSetResourceIgnoreDifferences>**](v1alpha1ApplicationSetResourceIgnoreDifferences.md)> |  | [optional]
**preserved_fields** | Option<[**models::V1alpha1ApplicationPreservedFields**](v1alpha1ApplicationPreservedFields.md)> |  | [optional]
**strategy** | Option<[**models::V1alpha1ApplicationSetStrategy**](v1alpha1ApplicationSetStrategy.md)> |  | [optional]
**sync_policy** | Option<[**models::V1alpha1ApplicationSetSyncPolicy**](v1alpha1ApplicationSetSyncPolicy.md)> |  | [optional]
**template** | Option<[**models::V1alpha1ApplicationSetTemplate**](v1alpha1ApplicationSetTemplate.md)> |  | [optional]
**template_patch** | Option<**String**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


