# V1Event

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**action** | Option<**String**> |  | [optional]
**count** | Option<**i32**> |  | [optional]
**event_time** | Option<[**models::V1MicroTime**](v1MicroTime.md)> |  | [optional]
**first_timestamp** | Option<**String**> | Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers.  +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false | [optional]
**involved_object** | Option<[**models::V1ObjectReference**](v1ObjectReference.md)> |  | [optional]
**last_timestamp** | Option<**String**> | Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers.  +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false | [optional]
**message** | Option<**String**> |  | [optional]
**metadata** | Option<[**models::V1ObjectMeta**](v1ObjectMeta.md)> |  | [optional]
**reason** | Option<**String**> |  | [optional]
**related** | Option<[**models::V1ObjectReference**](v1ObjectReference.md)> |  | [optional]
**reporting_component** | Option<**String**> |  | [optional]
**reporting_instance** | Option<**String**> |  | [optional]
**series** | Option<[**models::V1EventSeries**](v1EventSeries.md)> |  | [optional]
**source** | Option<[**models::V1EventSource**](v1EventSource.md)> |  | [optional]
**r#type** | Option<**String**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


