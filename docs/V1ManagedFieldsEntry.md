# V1ManagedFieldsEntry

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_version** | Option<**String**> | APIVersion defines the version of this resource that this field set applies to. The format is \"group/version\" just like the top-level APIVersion field. It is necessary to track the version of a field set because it cannot be automatically converted. | [optional]
**fields_type** | Option<**String**> |  | [optional]
**fields_v1** | Option<[**models::V1FieldsV1**](v1FieldsV1.md)> |  | [optional]
**manager** | Option<**String**> | Manager is an identifier of the workflow managing these fields. | [optional]
**operation** | Option<**String**> | Operation is the type of operation which lead to this ManagedFieldsEntry being created. The only valid values for this field are 'Apply' and 'Update'. | [optional]
**subresource** | Option<**String**> | Subresource is the name of the subresource used to update that object, or empty string if the object was updated through the main resource. The value of this field is used to distinguish between managers, even if they share the same name. For example, a status update will be distinct from a regular update using the same manager name. Note that the APIVersion field is not related to the Subresource field and it always corresponds to the version of the main resource. | [optional]
**time** | Option<**String**> | Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers.  +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


