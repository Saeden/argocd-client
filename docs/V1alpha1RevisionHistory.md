# V1alpha1RevisionHistory

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**deploy_started_at** | Option<**String**> | Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers.  +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false | [optional]
**deployed_at** | Option<**String**> | Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers.  +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false | [optional]
**id** | Option<**i64**> |  | [optional]
**initiated_by** | Option<[**models::V1alpha1OperationInitiator**](v1alpha1OperationInitiator.md)> |  | [optional]
**revision** | Option<**String**> |  | [optional]
**revisions** | Option<**Vec<String>**> |  | [optional]
**source** | Option<[**models::V1alpha1ApplicationSource**](v1alpha1ApplicationSource.md)> |  | [optional]
**sources** | Option<[**Vec<models::V1alpha1ApplicationSource>**](v1alpha1ApplicationSource.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


