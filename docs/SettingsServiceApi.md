# \SettingsServiceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**settings_service_get**](SettingsServiceApi.md#settings_service_get) | **GET** /api/v1/settings | Get returns Argo CD settings
[**settings_service_get_plugins**](SettingsServiceApi.md#settings_service_get_plugins) | **GET** /api/v1/settings/plugins | Get returns Argo CD plugins



## settings_service_get

> models::ClusterSettings settings_service_get()
Get returns Argo CD settings

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::ClusterSettings**](clusterSettings.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## settings_service_get_plugins

> models::ClusterSettingsPluginsResponse settings_service_get_plugins()
Get returns Argo CD plugins

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::ClusterSettingsPluginsResponse**](clusterSettingsPluginsResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

