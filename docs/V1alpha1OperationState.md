# V1alpha1OperationState

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**finished_at** | Option<**String**> | Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers.  +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false | [optional]
**message** | Option<**String**> | Message holds any pertinent messages when attempting to perform operation (typically errors). | [optional]
**operation** | Option<[**models::V1alpha1Operation**](v1alpha1Operation.md)> |  | [optional]
**phase** | Option<**String**> |  | [optional]
**retry_count** | Option<**i64**> |  | [optional]
**started_at** | Option<**String**> | Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers.  +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false | [optional]
**sync_result** | Option<[**models::V1alpha1SyncOperationResult**](v1alpha1SyncOperationResult.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


