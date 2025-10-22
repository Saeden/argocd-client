# \CertificateServiceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**certificate_service_create_certificate**](CertificateServiceApi.md#certificate_service_create_certificate) | **POST** /api/v1/certificates | Creates repository certificates on the server
[**certificate_service_delete_certificate**](CertificateServiceApi.md#certificate_service_delete_certificate) | **DELETE** /api/v1/certificates | Delete the certificates that match the RepositoryCertificateQuery
[**certificate_service_list_certificates**](CertificateServiceApi.md#certificate_service_list_certificates) | **GET** /api/v1/certificates | List all available repository certificates



## certificate_service_create_certificate

> models::V1alpha1RepositoryCertificateList certificate_service_create_certificate(body, upsert)
Creates repository certificates on the server

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1RepositoryCertificateList**](V1alpha1RepositoryCertificateList.md) | List of certificates to be created | [required] |
**upsert** | Option<**bool**> | Whether to upsert already existing certificates. |  |

### Return type

[**models::V1alpha1RepositoryCertificateList**](v1alpha1RepositoryCertificateList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## certificate_service_delete_certificate

> models::V1alpha1RepositoryCertificateList certificate_service_delete_certificate(host_name_pattern, cert_type, cert_sub_type)
Delete the certificates that match the RepositoryCertificateQuery

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**host_name_pattern** | Option<**String**> | A file-glob pattern (not regular expression) the host name has to match. |  |
**cert_type** | Option<**String**> | The type of the certificate to match (ssh or https). |  |
**cert_sub_type** | Option<**String**> | The sub type of the certificate to match (protocol dependent, usually only used for ssh certs). |  |

### Return type

[**models::V1alpha1RepositoryCertificateList**](v1alpha1RepositoryCertificateList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## certificate_service_list_certificates

> models::V1alpha1RepositoryCertificateList certificate_service_list_certificates(host_name_pattern, cert_type, cert_sub_type)
List all available repository certificates

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**host_name_pattern** | Option<**String**> | A file-glob pattern (not regular expression) the host name has to match. |  |
**cert_type** | Option<**String**> | The type of the certificate to match (ssh or https). |  |
**cert_sub_type** | Option<**String**> | The sub type of the certificate to match (protocol dependent, usually only used for ssh certs). |  |

### Return type

[**models::V1alpha1RepositoryCertificateList**](v1alpha1RepositoryCertificateList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

