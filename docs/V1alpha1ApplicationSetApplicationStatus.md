# V1alpha1ApplicationSetApplicationStatus

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**application** | Option<**String**> |  | [optional]
**last_transition_time** | Option<**String**> | Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers.  +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false | [optional]
**message** | Option<**String**> |  | [optional]
**status** | Option<**String**> |  | [optional]
**step** | Option<**String**> |  | [optional]
**targetrevisions** | Option<**Vec<String>**> | TargetRevision tracks the desired revisions the Application should be synced to. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


