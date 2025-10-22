# \SessionServiceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**session_service_create**](SessionServiceApi.md#session_service_create) | **POST** /api/v1/session | Create a new JWT for authentication and set a cookie if using HTTP
[**session_service_delete**](SessionServiceApi.md#session_service_delete) | **DELETE** /api/v1/session | Delete an existing JWT cookie if using HTTP
[**session_service_get_user_info**](SessionServiceApi.md#session_service_get_user_info) | **GET** /api/v1/session/userinfo | Get the current user's info



## session_service_create

> models::SessionSessionResponse session_service_create(body)
Create a new JWT for authentication and set a cookie if using HTTP

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**SessionSessionCreateRequest**](SessionSessionCreateRequest.md) |  | [required] |

### Return type

[**models::SessionSessionResponse**](sessionSessionResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## session_service_delete

> models::SessionSessionResponse session_service_delete()
Delete an existing JWT cookie if using HTTP

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::SessionSessionResponse**](sessionSessionResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## session_service_get_user_info

> models::SessionGetUserInfoResponse session_service_get_user_info()
Get the current user's info

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::SessionGetUserInfoResponse**](sessionGetUserInfoResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

