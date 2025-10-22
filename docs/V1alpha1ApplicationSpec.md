# V1alpha1ApplicationSpec

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**destination** | Option<[**models::V1alpha1ApplicationDestination**](v1alpha1ApplicationDestination.md)> |  | [optional]
**ignore_differences** | Option<[**Vec<models::V1alpha1ResourceIgnoreDifferences>**](v1alpha1ResourceIgnoreDifferences.md)> |  | [optional]
**info** | Option<[**Vec<models::V1alpha1Info>**](v1alpha1Info.md)> |  | [optional]
**project** | Option<**String**> | Project is a reference to the project this application belongs to. The empty string means that application belongs to the 'default' project. | [optional]
**revision_history_limit** | Option<**i64**> | RevisionHistoryLimit limits the number of items kept in the application's revision history, which is used for informational purposes as well as for rollbacks to previous versions. This should only be changed in exceptional circumstances. Setting to zero will store no history. This will reduce storage used. Increasing will increase the space used to store the history, so we do not recommend increasing it. Default is 10. | [optional]
**source** | Option<[**models::V1alpha1ApplicationSource**](v1alpha1ApplicationSource.md)> |  | [optional]
**source_hydrator** | Option<[**models::V1alpha1SourceHydrator**](v1alpha1SourceHydrator.md)> |  | [optional]
**sources** | Option<[**Vec<models::V1alpha1ApplicationSource>**](v1alpha1ApplicationSource.md)> |  | [optional]
**sync_policy** | Option<[**models::V1alpha1SyncPolicy**](v1alpha1SyncPolicy.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


