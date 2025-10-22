# V1alpha1ApplicationStatus

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conditions** | Option<[**Vec<models::V1alpha1ApplicationCondition>**](v1alpha1ApplicationCondition.md)> |  | [optional]
**controller_namespace** | Option<**String**> |  | [optional]
**health** | Option<[**models::V1alpha1AppHealthStatus**](v1alpha1AppHealthStatus.md)> |  | [optional]
**history** | Option<[**Vec<models::V1alpha1RevisionHistory>**](v1alpha1RevisionHistory.md)> |  | [optional]
**observed_at** | Option<**String**> | Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers.  +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false | [optional]
**operation_state** | Option<[**models::V1alpha1OperationState**](v1alpha1OperationState.md)> |  | [optional]
**reconciled_at** | Option<**String**> | Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers.  +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false | [optional]
**resource_health_source** | Option<**String**> |  | [optional]
**resources** | Option<[**Vec<models::Applicationv1alpha1ResourceStatus>**](applicationv1alpha1ResourceStatus.md)> |  | [optional]
**source_hydrator** | Option<[**models::V1alpha1SourceHydratorStatus**](v1alpha1SourceHydratorStatus.md)> |  | [optional]
**source_type** | Option<**String**> |  | [optional]
**source_types** | Option<**Vec<String>**> |  | [optional]
**summary** | Option<[**models::V1alpha1ApplicationSummary**](v1alpha1ApplicationSummary.md)> |  | [optional]
**sync** | Option<[**models::V1alpha1SyncStatus**](v1alpha1SyncStatus.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


