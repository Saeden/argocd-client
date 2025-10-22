# V1alpha1AppProjectSpec

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**cluster_resource_blacklist** | Option<[**Vec<models::V1GroupKind>**](v1GroupKind.md)> |  | [optional]
**cluster_resource_whitelist** | Option<[**Vec<models::V1GroupKind>**](v1GroupKind.md)> |  | [optional]
**description** | Option<**String**> |  | [optional]
**destination_service_accounts** | Option<[**Vec<models::V1alpha1ApplicationDestinationServiceAccount>**](v1alpha1ApplicationDestinationServiceAccount.md)> | DestinationServiceAccounts holds information about the service accounts to be impersonated for the application sync operation for each destination. | [optional]
**destinations** | Option<[**Vec<models::V1alpha1ApplicationDestination>**](v1alpha1ApplicationDestination.md)> |  | [optional]
**namespace_resource_blacklist** | Option<[**Vec<models::V1GroupKind>**](v1GroupKind.md)> |  | [optional]
**namespace_resource_whitelist** | Option<[**Vec<models::V1GroupKind>**](v1GroupKind.md)> |  | [optional]
**orphaned_resources** | Option<[**models::V1alpha1OrphanedResourcesMonitorSettings**](v1alpha1OrphanedResourcesMonitorSettings.md)> |  | [optional]
**permit_only_project_scoped_clusters** | Option<**bool**> |  | [optional]
**roles** | Option<[**Vec<models::V1alpha1ProjectRole>**](v1alpha1ProjectRole.md)> |  | [optional]
**signature_keys** | Option<[**Vec<models::V1alpha1SignatureKey>**](v1alpha1SignatureKey.md)> |  | [optional]
**source_namespaces** | Option<**Vec<String>**> |  | [optional]
**source_repos** | Option<**Vec<String>**> |  | [optional]
**sync_windows** | Option<[**Vec<models::V1alpha1SyncWindow>**](v1alpha1SyncWindow.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


