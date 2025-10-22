# V1alpha1ClusterConfig

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**aws_auth_config** | Option<[**models::V1alpha1AwsAuthConfig**](v1alpha1AWSAuthConfig.md)> |  | [optional]
**bearer_token** | Option<**String**> | Server requires Bearer authentication. This client will not attempt to use refresh tokens for an OAuth2 flow. TODO: demonstrate an OAuth2 compatible client. | [optional]
**disable_compression** | Option<**bool**> | DisableCompression bypasses automatic GZip compression requests to the server. | [optional]
**exec_provider_config** | Option<[**models::V1alpha1ExecProviderConfig**](v1alpha1ExecProviderConfig.md)> |  | [optional]
**password** | Option<**String**> |  | [optional]
**proxy_url** | Option<**String**> |  | [optional]
**tls_client_config** | Option<[**models::V1alpha1TlsClientConfig**](v1alpha1TLSClientConfig.md)> |  | [optional]
**username** | Option<**String**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


