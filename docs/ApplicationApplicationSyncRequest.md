# ApplicationApplicationSyncRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app_namespace** | Option<**String**> |  | [optional]
**dry_run** | Option<**bool**> |  | [optional]
**infos** | Option<[**Vec<models::V1alpha1Info>**](v1alpha1Info.md)> |  | [optional]
**manifests** | Option<**Vec<String>**> |  | [optional]
**name** | Option<**String**> |  | [optional]
**project** | Option<**String**> |  | [optional]
**prune** | Option<**bool**> |  | [optional]
**resources** | Option<[**Vec<models::V1alpha1SyncOperationResource>**](v1alpha1SyncOperationResource.md)> |  | [optional]
**retry_strategy** | Option<[**models::V1alpha1RetryStrategy**](v1alpha1RetryStrategy.md)> |  | [optional]
**revision** | Option<**String**> |  | [optional]
**revisions** | Option<**Vec<String>**> |  | [optional]
**source_positions** | Option<**Vec<String>**> |  | [optional]
**strategy** | Option<[**models::V1alpha1SyncStrategy**](v1alpha1SyncStrategy.md)> |  | [optional]
**sync_options** | Option<[**models::ApplicationSyncOptions**](applicationSyncOptions.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


