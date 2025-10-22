# V1alpha1TlsClientConfig

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ca_data** | Option<**String**> |  | [optional]
**cert_data** | Option<**String**> |  | [optional]
**insecure** | Option<**bool**> | Insecure specifies that the server should be accessed without verifying the TLS certificate. For testing only. | [optional]
**key_data** | Option<**String**> |  | [optional]
**server_name** | Option<**String**> | ServerName is passed to the server for SNI and is used in the client to check server certificates against. If ServerName is empty, the hostname used to contact the server is used. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


