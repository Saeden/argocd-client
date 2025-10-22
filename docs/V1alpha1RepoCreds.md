# V1alpha1RepoCreds

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bearer_token** | Option<**String**> |  | [optional]
**enable_oci** | Option<**bool**> |  | [optional]
**force_http_basic_auth** | Option<**bool**> |  | [optional]
**gcp_service_account_key** | Option<**String**> |  | [optional]
**github_app_enterprise_base_url** | Option<**String**> |  | [optional]
**github_app_id** | Option<**i64**> |  | [optional]
**github_app_installation_id** | Option<**i64**> |  | [optional]
**github_app_private_key** | Option<**String**> |  | [optional]
**insecure_oci_force_http** | Option<**bool**> | InsecureOCIForceHttp specifies whether the connection to the repository uses TLS at _all_. If true, no TLS. This flag is applicable for OCI repos only. | [optional]
**no_proxy** | Option<**String**> |  | [optional]
**password** | Option<**String**> |  | [optional]
**proxy** | Option<**String**> |  | [optional]
**ssh_private_key** | Option<**String**> |  | [optional]
**tls_client_cert_data** | Option<**String**> |  | [optional]
**tls_client_cert_key** | Option<**String**> |  | [optional]
**r#type** | Option<**String**> | Type specifies the type of the repoCreds. Can be either \"git\" or \"helm. \"git\" is assumed if empty or absent. | [optional]
**url** | Option<**String**> |  | [optional]
**use_azure_workload_identity** | Option<**bool**> |  | [optional]
**username** | Option<**String**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


