# Applicationv1alpha1ResourceStatus

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**group** | Option<**String**> | Group represents the API group of the resource (e.g., \"apps\" for Deployments). | [optional]
**health** | Option<[**models::V1alpha1HealthStatus**](v1alpha1HealthStatus.md)> |  | [optional]
**hook** | Option<**bool**> | Hook is true if the resource is used as a lifecycle hook in an Argo CD application. | [optional]
**kind** | Option<**String**> | Kind specifies the type of the resource (e.g., \"Deployment\", \"Service\"). | [optional]
**name** | Option<**String**> | Name is the unique name of the resource within the namespace. | [optional]
**namespace** | Option<**String**> | Namespace defines the Kubernetes namespace where the resource is located. | [optional]
**requires_deletion_confirmation** | Option<**bool**> | RequiresDeletionConfirmation is true if the resource requires explicit user confirmation before deletion. | [optional]
**requires_pruning** | Option<**bool**> | RequiresPruning is true if the resource needs to be pruned (deleted) as part of synchronization. | [optional]
**status** | Option<**String**> | Status represents the synchronization state of the resource (e.g., Synced, OutOfSync). | [optional]
**sync_wave** | Option<**i64**> | SyncWave determines the order in which resources are applied during a sync operation. Lower values are applied first. | [optional]
**version** | Option<**String**> | Version indicates the API version of the resource (e.g., \"v1\", \"v1beta1\"). | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


