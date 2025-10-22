# V1alpha1Repository

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bearer_token** | Option<**String**> |  | [optional]
**connection_state** | Option<[**models::V1alpha1ConnectionState**](v1alpha1ConnectionState.md)> |  | [optional]
**enable_lfs** | Option<**bool**> | EnableLFS specifies whether git-lfs support should be enabled for this repo. Only valid for Git repositories. | [optional]
**enable_oci** | Option<**bool**> |  | [optional]
**force_http_basic_auth** | Option<**bool**> |  | [optional]
**gcp_service_account_key** | Option<**String**> |  | [optional]
**github_app_enterprise_base_url** | Option<**String**> |  | [optional]
**github_app_id** | Option<**i64**> |  | [optional]
**github_app_installation_id** | Option<**i64**> |  | [optional]
**github_app_private_key** | Option<**String**> |  | [optional]
**inherited_creds** | Option<**bool**> |  | [optional]
**insecure** | Option<**bool**> |  | [optional]
**insecure_ignore_host_key** | Option<**bool**> |  | [optional]
**insecure_oci_force_http** | Option<**bool**> | InsecureOCIForceHttp specifies whether the connection to the repository uses TLS at _all_. If true, no TLS. This flag is applicable for OCI repos only. | [optional]
**name** | Option<**String**> |  | [optional]
**no_proxy** | Option<**String**> |  | [optional]
**password** | Option<**String**> |  | [optional]
**project** | Option<**String**> |  | [optional]
**proxy** | Option<**String**> |  | [optional]
**repo** | Option<**String**> |  | [optional]
**ssh_private_key** | Option<**String**> | SSHPrivateKey contains the PEM data for authenticating at the repo server. Only used with Git repos. | [optional]
**tls_client_cert_data** | Option<**String**> |  | [optional]
**tls_client_cert_key** | Option<**String**> |  | [optional]
**r#type** | Option<**String**> | Type specifies the type of the repo. Can be either \"git\" or \"helm. \"git\" is assumed if empty or absent. | [optional]
**use_azure_workload_identity** | Option<**bool**> |  | [optional]
**username** | Option<**String**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


