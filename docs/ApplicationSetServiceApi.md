# \ApplicationSetServiceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**application_set_service_create**](ApplicationSetServiceApi.md#application_set_service_create) | **POST** /api/v1/applicationsets | Create creates an applicationset
[**application_set_service_delete**](ApplicationSetServiceApi.md#application_set_service_delete) | **DELETE** /api/v1/applicationsets/{name} | Delete deletes an application set
[**application_set_service_generate**](ApplicationSetServiceApi.md#application_set_service_generate) | **POST** /api/v1/applicationsets/generate | Generate generates
[**application_set_service_get**](ApplicationSetServiceApi.md#application_set_service_get) | **GET** /api/v1/applicationsets/{name} | Get returns an applicationset by name
[**application_set_service_list**](ApplicationSetServiceApi.md#application_set_service_list) | **GET** /api/v1/applicationsets | List returns list of applicationset
[**application_set_service_resource_tree**](ApplicationSetServiceApi.md#application_set_service_resource_tree) | **GET** /api/v1/applicationsets/{name}/resource-tree | ResourceTree returns resource tree



## application_set_service_create

> models::V1alpha1ApplicationSet application_set_service_create(body, upsert, dry_run)
Create creates an applicationset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1ApplicationSet**](V1alpha1ApplicationSet.md) |  | [required] |
**upsert** | Option<**bool**> |  |  |
**dry_run** | Option<**bool**> |  |  |

### Return type

[**models::V1alpha1ApplicationSet**](v1alpha1ApplicationSet.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_set_service_delete

> models::ApplicationsetApplicationSetResponse application_set_service_delete(name, appset_namespace)
Delete deletes an application set

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**appset_namespace** | Option<**String**> | The application set namespace. Default empty is argocd control plane namespace. |  |

### Return type

[**models::ApplicationsetApplicationSetResponse**](applicationsetApplicationSetResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_set_service_generate

> models::ApplicationsetApplicationSetGenerateResponse application_set_service_generate(body)
Generate generates

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**ApplicationsetApplicationSetGenerateRequest**](ApplicationsetApplicationSetGenerateRequest.md) |  | [required] |

### Return type

[**models::ApplicationsetApplicationSetGenerateResponse**](applicationsetApplicationSetGenerateResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_set_service_get

> models::V1alpha1ApplicationSet application_set_service_get(name, appset_namespace)
Get returns an applicationset by name

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** | the applicationsets's name | [required] |
**appset_namespace** | Option<**String**> | The application set namespace. Default empty is argocd control plane namespace. |  |

### Return type

[**models::V1alpha1ApplicationSet**](v1alpha1ApplicationSet.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_set_service_list

> models::V1alpha1ApplicationSetList application_set_service_list(projects, selector, appset_namespace)
List returns list of applicationset

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**projects** | Option<[**Vec<String>**](String.md)> | the project names to restrict returned list applicationsets. |  |
**selector** | Option<**String**> | the selector to restrict returned list to applications only with matched labels. |  |
**appset_namespace** | Option<**String**> | The application set namespace. Default empty is argocd control plane namespace. |  |

### Return type

[**models::V1alpha1ApplicationSetList**](v1alpha1ApplicationSetList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_set_service_resource_tree

> models::V1alpha1ApplicationSetTree application_set_service_resource_tree(name, appset_namespace)
ResourceTree returns resource tree

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**appset_namespace** | Option<**String**> | The application set namespace. Default empty is argocd control plane namespace. |  |

### Return type

[**models::V1alpha1ApplicationSetTree**](v1alpha1ApplicationSetTree.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

