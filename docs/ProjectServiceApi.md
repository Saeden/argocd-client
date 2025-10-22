# \ProjectServiceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**project_service_create**](ProjectServiceApi.md#project_service_create) | **POST** /api/v1/projects | Create a new project
[**project_service_create_token**](ProjectServiceApi.md#project_service_create_token) | **POST** /api/v1/projects/{project}/roles/{role}/token | Create a new project token
[**project_service_delete**](ProjectServiceApi.md#project_service_delete) | **DELETE** /api/v1/projects/{name} | Delete deletes a project
[**project_service_delete_token**](ProjectServiceApi.md#project_service_delete_token) | **DELETE** /api/v1/projects/{project}/roles/{role}/token/{iat} | Delete a new project token
[**project_service_get**](ProjectServiceApi.md#project_service_get) | **GET** /api/v1/projects/{name} | Get returns a project by name
[**project_service_get_detailed_project**](ProjectServiceApi.md#project_service_get_detailed_project) | **GET** /api/v1/projects/{name}/detailed | GetDetailedProject returns a project that include project, global project and scoped resources by name
[**project_service_get_global_projects**](ProjectServiceApi.md#project_service_get_global_projects) | **GET** /api/v1/projects/{name}/globalprojects | Get returns a virtual project by name
[**project_service_get_sync_windows_state**](ProjectServiceApi.md#project_service_get_sync_windows_state) | **GET** /api/v1/projects/{name}/syncwindows | GetSchedulesState returns true if there are any active sync syncWindows
[**project_service_list**](ProjectServiceApi.md#project_service_list) | **GET** /api/v1/projects | List returns list of projects
[**project_service_list_events**](ProjectServiceApi.md#project_service_list_events) | **GET** /api/v1/projects/{name}/events | ListEvents returns a list of project events
[**project_service_list_links**](ProjectServiceApi.md#project_service_list_links) | **GET** /api/v1/projects/{name}/links | ListLinks returns all deep links for the particular project
[**project_service_update**](ProjectServiceApi.md#project_service_update) | **PUT** /api/v1/projects/{project.metadata.name} | Update updates a project



## project_service_create

> models::V1alpha1AppProject project_service_create(body)
Create a new project

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**ProjectProjectCreateRequest**](ProjectProjectCreateRequest.md) |  | [required] |

### Return type

[**models::V1alpha1AppProject**](v1alpha1AppProject.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## project_service_create_token

> models::ProjectProjectTokenResponse project_service_create_token(body, project, role)
Create a new project token

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**ProjectProjectTokenCreateRequest**](ProjectProjectTokenCreateRequest.md) |  | [required] |
**project** | **String** |  | [required] |
**role** | **String** |  | [required] |

### Return type

[**models::ProjectProjectTokenResponse**](projectProjectTokenResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## project_service_delete

> serde_json::Value project_service_delete(name)
Delete deletes a project

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## project_service_delete_token

> serde_json::Value project_service_delete_token(project, role, iat, id)
Delete a new project token

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project** | **String** |  | [required] |
**role** | **String** |  | [required] |
**iat** | **String** |  | [required] |
**id** | Option<**String**> |  |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## project_service_get

> models::V1alpha1AppProject project_service_get(name)
Get returns a project by name

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |

### Return type

[**models::V1alpha1AppProject**](v1alpha1AppProject.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## project_service_get_detailed_project

> models::ProjectDetailedProjectsResponse project_service_get_detailed_project(name)
GetDetailedProject returns a project that include project, global project and scoped resources by name

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |

### Return type

[**models::ProjectDetailedProjectsResponse**](projectDetailedProjectsResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## project_service_get_global_projects

> models::ProjectGlobalProjectsResponse project_service_get_global_projects(name)
Get returns a virtual project by name

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |

### Return type

[**models::ProjectGlobalProjectsResponse**](projectGlobalProjectsResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## project_service_get_sync_windows_state

> models::ProjectSyncWindowsResponse project_service_get_sync_windows_state(name)
GetSchedulesState returns true if there are any active sync syncWindows

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |

### Return type

[**models::ProjectSyncWindowsResponse**](projectSyncWindowsResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## project_service_list

> models::V1alpha1AppProjectList project_service_list(name)
List returns list of projects

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | Option<**String**> |  |  |

### Return type

[**models::V1alpha1AppProjectList**](v1alpha1AppProjectList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## project_service_list_events

> models::V1EventList project_service_list_events(name)
ListEvents returns a list of project events

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |

### Return type

[**models::V1EventList**](v1EventList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## project_service_list_links

> models::ApplicationLinksResponse project_service_list_links(name)
ListLinks returns all deep links for the particular project

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |

### Return type

[**models::ApplicationLinksResponse**](applicationLinksResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## project_service_update

> models::V1alpha1AppProject project_service_update(body, project_metadata_name)
Update updates a project

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**ProjectProjectUpdateRequest**](ProjectProjectUpdateRequest.md) |  | [required] |
**project_metadata_name** | **String** | Name must be unique within a namespace. Is required when creating resources, although some resources may allow a client to request the generation of an appropriate name automatically. Name is primarily intended for creation idempotence and configuration definition. Cannot be updated. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names#names +optional | [required] |

### Return type

[**models::V1alpha1AppProject**](v1alpha1AppProject.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

