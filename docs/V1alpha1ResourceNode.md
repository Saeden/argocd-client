# V1alpha1ResourceNode

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | Option<**String**> | Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers.  +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false | [optional]
**health** | Option<[**models::V1alpha1HealthStatus**](v1alpha1HealthStatus.md)> |  | [optional]
**images** | Option<**Vec<String>**> | Images lists container images associated with the resource. This is primarily useful for pods and other workload resources. | [optional]
**info** | Option<[**Vec<models::V1alpha1InfoItem>**](v1alpha1InfoItem.md)> | Info provides additional metadata or annotations about the resource. | [optional]
**networking_info** | Option<[**models::V1alpha1ResourceNetworkingInfo**](v1alpha1ResourceNetworkingInfo.md)> |  | [optional]
**parent_refs** | Option<[**Vec<models::V1alpha1ResourceRef>**](v1alpha1ResourceRef.md)> | ParentRefs lists the parent resources that reference this resource. This helps in understanding ownership and hierarchical relationships. | [optional]
**resource_version** | Option<**String**> | ResourceVersion indicates the version of the resource, used to track changes. | [optional]
**group** | Option<**String**> |  | [optional]
**kind** | Option<**String**> |  | [optional]
**name** | Option<**String**> |  | [optional]
**namespace** | Option<**String**> |  | [optional]
**uid** | Option<**String**> |  | [optional]
**version** | Option<**String**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


