# \GpgKeyServiceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**g_pg_key_service_create**](GpgKeyServiceApi.md#g_pg_key_service_create) | **POST** /api/v1/gpgkeys | Create one or more GPG public keys in the server's configuration
[**g_pg_key_service_delete**](GpgKeyServiceApi.md#g_pg_key_service_delete) | **DELETE** /api/v1/gpgkeys | Delete specified GPG public key from the server's configuration
[**g_pg_key_service_get**](GpgKeyServiceApi.md#g_pg_key_service_get) | **GET** /api/v1/gpgkeys/{keyID} | Get information about specified GPG public key from the server
[**g_pg_key_service_list**](GpgKeyServiceApi.md#g_pg_key_service_list) | **GET** /api/v1/gpgkeys | List all available repository certificates



## g_pg_key_service_create

> models::GpgkeyGnuPgPublicKeyCreateResponse g_pg_key_service_create(body, upsert)
Create one or more GPG public keys in the server's configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1GnuPgPublicKey**](V1alpha1GnuPgPublicKey.md) | Raw key data of the GPG key(s) to create | [required] |
**upsert** | Option<**bool**> | Whether to upsert already existing public keys. |  |

### Return type

[**models::GpgkeyGnuPgPublicKeyCreateResponse**](gpgkeyGnuPGPublicKeyCreateResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## g_pg_key_service_delete

> serde_json::Value g_pg_key_service_delete(key_id)
Delete specified GPG public key from the server's configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**key_id** | Option<**String**> | The GPG key ID to query for. |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## g_pg_key_service_get

> models::V1alpha1GnuPgPublicKey g_pg_key_service_get(key_id)
Get information about specified GPG public key from the server

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**key_id** | **String** | The GPG key ID to query for | [required] |

### Return type

[**models::V1alpha1GnuPgPublicKey**](v1alpha1GnuPGPublicKey.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## g_pg_key_service_list

> models::V1alpha1GnuPgPublicKeyList g_pg_key_service_list(key_id)
List all available repository certificates

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**key_id** | Option<**String**> | The GPG key ID to query for. |  |

### Return type

[**models::V1alpha1GnuPgPublicKeyList**](v1alpha1GnuPGPublicKeyList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

