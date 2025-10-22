# V1alpha1SyncOperation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**auto_heal_attempts_count** | Option<**i64**> |  | [optional]
**dry_run** | Option<**bool**> |  | [optional]
**manifests** | Option<**Vec<String>**> |  | [optional]
**prune** | Option<**bool**> |  | [optional]
**resources** | Option<[**Vec<models::V1alpha1SyncOperationResource>**](v1alpha1SyncOperationResource.md)> |  | [optional]
**revision** | Option<**String**> | Revision is the revision (Git) or chart version (Helm) which to sync the application to If omitted, will use the revision specified in app spec. | [optional]
**revisions** | Option<**Vec<String>**> | Revisions is the list of revision (Git) or chart version (Helm) which to sync each source in sources field for the application to If omitted, will use the revision specified in app spec. | [optional]
**source** | Option<[**models::V1alpha1ApplicationSource**](v1alpha1ApplicationSource.md)> |  | [optional]
**sources** | Option<[**Vec<models::V1alpha1ApplicationSource>**](v1alpha1ApplicationSource.md)> |  | [optional]
**sync_options** | Option<**Vec<String>**> |  | [optional]
**sync_strategy** | Option<[**models::V1alpha1SyncStrategy**](v1alpha1SyncStrategy.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


