# V1alpha1HostResourceInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**capacity** | Option<**i64**> | Capacity represents the total available capacity of this resource on the host. | [optional]
**requested_by_app** | Option<**i64**> | RequestedByApp indicates the total amount of this resource requested by the application running on the host. | [optional]
**requested_by_neighbors** | Option<**i64**> | RequestedByNeighbors indicates the total amount of this resource requested by other workloads on the same host. | [optional]
**resource_name** | Option<**String**> | ResourceName specifies the type of resource (e.g., CPU, memory, storage). | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


