# \ClusterServiceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cluster_service_create**](ClusterServiceApi.md#cluster_service_create) | **POST** /api/v1/clusters | Create creates a cluster
[**cluster_service_delete**](ClusterServiceApi.md#cluster_service_delete) | **DELETE** /api/v1/clusters/{id.value} | Delete deletes a cluster
[**cluster_service_get**](ClusterServiceApi.md#cluster_service_get) | **GET** /api/v1/clusters/{id.value} | Get returns a cluster by server address
[**cluster_service_invalidate_cache**](ClusterServiceApi.md#cluster_service_invalidate_cache) | **POST** /api/v1/clusters/{id.value}/invalidate-cache | InvalidateCache invalidates cluster cache
[**cluster_service_list**](ClusterServiceApi.md#cluster_service_list) | **GET** /api/v1/clusters | List returns list of clusters
[**cluster_service_rotate_auth**](ClusterServiceApi.md#cluster_service_rotate_auth) | **POST** /api/v1/clusters/{id.value}/rotate-auth | RotateAuth rotates the bearer token used for a cluster
[**cluster_service_update**](ClusterServiceApi.md#cluster_service_update) | **PUT** /api/v1/clusters/{id.value} | Update updates a cluster



## cluster_service_create

> models::V1alpha1Cluster cluster_service_create(body, upsert)
Create creates a cluster

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1Cluster**](V1alpha1Cluster.md) |  | [required] |
**upsert** | Option<**bool**> |  |  |

### Return type

[**models::V1alpha1Cluster**](v1alpha1Cluster.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## cluster_service_delete

> serde_json::Value cluster_service_delete(id_value, server, name, id_type)
Delete deletes a cluster

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id_value** | **String** | value holds the cluster server URL or cluster name | [required] |
**server** | Option<**String**> |  |  |
**name** | Option<**String**> |  |  |
**id_type** | Option<**String**> | type is the type of the specified cluster identifier ( \"server\" - default, \"name\" ). |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## cluster_service_get

> models::V1alpha1Cluster cluster_service_get(id_value, server, name, id_type)
Get returns a cluster by server address

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id_value** | **String** | value holds the cluster server URL or cluster name | [required] |
**server** | Option<**String**> |  |  |
**name** | Option<**String**> |  |  |
**id_type** | Option<**String**> | type is the type of the specified cluster identifier ( \"server\" - default, \"name\" ). |  |

### Return type

[**models::V1alpha1Cluster**](v1alpha1Cluster.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## cluster_service_invalidate_cache

> models::V1alpha1Cluster cluster_service_invalidate_cache(id_value)
InvalidateCache invalidates cluster cache

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id_value** | **String** | value holds the cluster server URL or cluster name | [required] |

### Return type

[**models::V1alpha1Cluster**](v1alpha1Cluster.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## cluster_service_list

> models::V1alpha1ClusterList cluster_service_list(server, name, id_type, id_value)
List returns list of clusters

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**server** | Option<**String**> |  |  |
**name** | Option<**String**> |  |  |
**id_type** | Option<**String**> | type is the type of the specified cluster identifier ( \"server\" - default, \"name\" ). |  |
**id_value** | Option<**String**> | value holds the cluster server URL or cluster name. |  |

### Return type

[**models::V1alpha1ClusterList**](v1alpha1ClusterList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## cluster_service_rotate_auth

> serde_json::Value cluster_service_rotate_auth(id_value)
RotateAuth rotates the bearer token used for a cluster

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id_value** | **String** | value holds the cluster server URL or cluster name | [required] |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## cluster_service_update

> models::V1alpha1Cluster cluster_service_update(body, id_value, updated_fields, id_type)
Update updates a cluster

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1Cluster**](V1alpha1Cluster.md) |  | [required] |
**id_value** | **String** | value holds the cluster server URL or cluster name | [required] |
**updated_fields** | Option<[**Vec<String>**](String.md)> |  |  |
**id_type** | Option<**String**> | type is the type of the specified cluster identifier ( \"server\" - default, \"name\" ). |  |

### Return type

[**models::V1alpha1Cluster**](v1alpha1Cluster.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

