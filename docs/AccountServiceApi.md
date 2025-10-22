# \AccountServiceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**account_service_can_i**](AccountServiceApi.md#account_service_can_i) | **GET** /api/v1/account/can-i/{resource}/{action}/{subresource} | CanI checks if the current account has permission to perform an action
[**account_service_create_token**](AccountServiceApi.md#account_service_create_token) | **POST** /api/v1/account/{name}/token | CreateToken creates a token
[**account_service_delete_token**](AccountServiceApi.md#account_service_delete_token) | **DELETE** /api/v1/account/{name}/token/{id} | DeleteToken deletes a token
[**account_service_get_account**](AccountServiceApi.md#account_service_get_account) | **GET** /api/v1/account/{name} | GetAccount returns an account
[**account_service_list_accounts**](AccountServiceApi.md#account_service_list_accounts) | **GET** /api/v1/account | ListAccounts returns the list of accounts
[**account_service_update_password**](AccountServiceApi.md#account_service_update_password) | **PUT** /api/v1/account/password | UpdatePassword updates an account's password to a new value



## account_service_can_i

> models::AccountCanIResponse account_service_can_i(resource, action, subresource)
CanI checks if the current account has permission to perform an action

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**resource** | **String** |  | [required] |
**action** | **String** |  | [required] |
**subresource** | **String** |  | [required] |

### Return type

[**models::AccountCanIResponse**](accountCanIResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## account_service_create_token

> models::AccountCreateTokenResponse account_service_create_token(body, name)
CreateToken creates a token

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**AccountCreateTokenRequest**](AccountCreateTokenRequest.md) |  | [required] |
**name** | **String** |  | [required] |

### Return type

[**models::AccountCreateTokenResponse**](accountCreateTokenResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## account_service_delete_token

> serde_json::Value account_service_delete_token(name, id)
DeleteToken deletes a token

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**id** | **String** |  | [required] |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## account_service_get_account

> models::AccountAccount account_service_get_account(name)
GetAccount returns an account

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |

### Return type

[**models::AccountAccount**](accountAccount.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## account_service_list_accounts

> models::AccountAccountsList account_service_list_accounts()
ListAccounts returns the list of accounts

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::AccountAccountsList**](accountAccountsList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## account_service_update_password

> serde_json::Value account_service_update_password(body)
UpdatePassword updates an account's password to a new value

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**AccountUpdatePasswordRequest**](AccountUpdatePasswordRequest.md) |  | [required] |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

