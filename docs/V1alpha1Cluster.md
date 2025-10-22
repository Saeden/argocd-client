# V1alpha1Cluster

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**annotations** | Option<**std::collections::HashMap<String, String>**> |  | [optional]
**cluster_resources** | Option<**bool**> | Indicates if cluster level resources should be managed. This setting is used only if cluster is connected in a namespaced mode. | [optional]
**config** | Option<[**models::V1alpha1ClusterConfig**](v1alpha1ClusterConfig.md)> |  | [optional]
**connection_state** | Option<[**models::V1alpha1ConnectionState**](v1alpha1ConnectionState.md)> |  | [optional]
**info** | Option<[**models::V1alpha1ClusterInfo**](v1alpha1ClusterInfo.md)> |  | [optional]
**labels** | Option<**std::collections::HashMap<String, String>**> |  | [optional]
**name** | Option<**String**> |  | [optional]
**namespaces** | Option<**Vec<String>**> | Holds list of namespaces which are accessible in that cluster. Cluster level resources will be ignored if namespace list is not empty. | [optional]
**project** | Option<**String**> |  | [optional]
**refresh_requested_at** | Option<**String**> | Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers.  +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false | [optional]
**server** | Option<**String**> |  | [optional]
**server_version** | Option<**String**> |  | [optional]
**shard** | Option<**i64**> | Shard contains optional shard number. Calculated on the fly by the application controller if not specified. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


