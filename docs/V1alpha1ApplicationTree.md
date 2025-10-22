# V1alpha1ApplicationTree

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**hosts** | Option<[**Vec<models::V1alpha1HostInfo>**](v1alpha1HostInfo.md)> | Hosts provides a list of Kubernetes nodes that are running pods related to the application. | [optional]
**nodes** | Option<[**Vec<models::V1alpha1ResourceNode>**](v1alpha1ResourceNode.md)> | Nodes contains a list of resources that are either directly managed by the application or are children of directly managed resources. | [optional]
**orphaned_nodes** | Option<[**Vec<models::V1alpha1ResourceNode>**](v1alpha1ResourceNode.md)> | OrphanedNodes contains resources that exist in the same namespace as the application but are not managed by it. This list is populated only if orphaned resource tracking is enabled in the application's project settings. | [optional]
**shards_count** | Option<**i64**> | ShardsCount represents the total number of shards the application tree is split into. This is used to distribute resource processing across multiple shards. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


