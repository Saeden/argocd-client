# V1alpha1RevisionMetadata

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**author** | Option<**String**> |  | [optional]
**date** | Option<**String**> | Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers.  +protobuf.options.marshal=false +protobuf.as=Timestamp +protobuf.options.(gogoproto.goproto_stringer)=false | [optional]
**message** | Option<**String**> | Message contains the message associated with the revision, most likely the commit message. | [optional]
**references** | Option<[**Vec<models::V1alpha1RevisionReference>**](v1alpha1RevisionReference.md)> | References contains references to information that's related to this commit in some way. | [optional]
**signature_info** | Option<**String**> | SignatureInfo contains a hint on the signer if the revision was signed with GPG, and signature verification is enabled. | [optional]
**tags** | Option<**Vec<String>**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


