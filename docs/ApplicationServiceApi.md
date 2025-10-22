# \ApplicationServiceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**application_service_create**](ApplicationServiceApi.md#application_service_create) | **POST** /api/v1/applications | Create creates an application
[**application_service_delete**](ApplicationServiceApi.md#application_service_delete) | **DELETE** /api/v1/applications/{name} | Delete deletes an application
[**application_service_delete_resource**](ApplicationServiceApi.md#application_service_delete_resource) | **DELETE** /api/v1/applications/{name}/resource | DeleteResource deletes a single application resource
[**application_service_get**](ApplicationServiceApi.md#application_service_get) | **GET** /api/v1/applications/{name} | Get returns an application by name
[**application_service_get_application_sync_windows**](ApplicationServiceApi.md#application_service_get_application_sync_windows) | **GET** /api/v1/applications/{name}/syncwindows | Get returns sync windows of the application
[**application_service_get_manifests**](ApplicationServiceApi.md#application_service_get_manifests) | **GET** /api/v1/applications/{name}/manifests | GetManifests returns application manifests
[**application_service_get_manifests_with_files**](ApplicationServiceApi.md#application_service_get_manifests_with_files) | **POST** /api/v1/applications/manifestsWithFiles | GetManifestsWithFiles returns application manifests using provided files to generate them
[**application_service_get_oci_metadata**](ApplicationServiceApi.md#application_service_get_oci_metadata) | **GET** /api/v1/applications/{name}/revisions/{revision}/ocimetadata | Get the chart metadata (description, maintainers, home) for a specific revision of the application
[**application_service_get_resource**](ApplicationServiceApi.md#application_service_get_resource) | **GET** /api/v1/applications/{name}/resource | GetResource returns single application resource
[**application_service_list**](ApplicationServiceApi.md#application_service_list) | **GET** /api/v1/applications | List returns list of applications
[**application_service_list_links**](ApplicationServiceApi.md#application_service_list_links) | **GET** /api/v1/applications/{name}/links | ListLinks returns the list of all application deep links
[**application_service_list_resource_actions**](ApplicationServiceApi.md#application_service_list_resource_actions) | **GET** /api/v1/applications/{name}/resource/actions | ListResourceActions returns list of resource actions
[**application_service_list_resource_events**](ApplicationServiceApi.md#application_service_list_resource_events) | **GET** /api/v1/applications/{name}/events | ListResourceEvents returns a list of event resources
[**application_service_list_resource_links**](ApplicationServiceApi.md#application_service_list_resource_links) | **GET** /api/v1/applications/{name}/resource/links | ListResourceLinks returns the list of all resource deep links
[**application_service_managed_resources**](ApplicationServiceApi.md#application_service_managed_resources) | **GET** /api/v1/applications/{applicationName}/managed-resources | ManagedResources returns list of managed resources
[**application_service_patch**](ApplicationServiceApi.md#application_service_patch) | **PATCH** /api/v1/applications/{name} | Patch patch an application
[**application_service_patch_resource**](ApplicationServiceApi.md#application_service_patch_resource) | **POST** /api/v1/applications/{name}/resource | PatchResource patch single application resource
[**application_service_pod_logs**](ApplicationServiceApi.md#application_service_pod_logs) | **GET** /api/v1/applications/{name}/pods/{podName}/logs | PodLogs returns stream of log entries for the specified pod. Pod
[**application_service_pod_logs2**](ApplicationServiceApi.md#application_service_pod_logs2) | **GET** /api/v1/applications/{name}/logs | PodLogs returns stream of log entries for the specified pod. Pod
[**application_service_resource_tree**](ApplicationServiceApi.md#application_service_resource_tree) | **GET** /api/v1/applications/{applicationName}/resource-tree | ResourceTree returns resource tree
[**application_service_revision_chart_details**](ApplicationServiceApi.md#application_service_revision_chart_details) | **GET** /api/v1/applications/{name}/revisions/{revision}/chartdetails | Get the chart metadata (description, maintainers, home) for a specific revision of the application
[**application_service_revision_metadata**](ApplicationServiceApi.md#application_service_revision_metadata) | **GET** /api/v1/applications/{name}/revisions/{revision}/metadata | Get the meta-data (author, date, tags, message) for a specific revision of the application
[**application_service_rollback**](ApplicationServiceApi.md#application_service_rollback) | **POST** /api/v1/applications/{name}/rollback | Rollback syncs an application to its target state
[**application_service_run_resource_action**](ApplicationServiceApi.md#application_service_run_resource_action) | **POST** /api/v1/applications/{name}/resource/actions | RunResourceAction runs a resource action
[**application_service_run_resource_action_v2**](ApplicationServiceApi.md#application_service_run_resource_action_v2) | **POST** /api/v1/applications/{name}/resource/actions/v2 | RunResourceActionV2 runs a resource action with parameters
[**application_service_sync**](ApplicationServiceApi.md#application_service_sync) | **POST** /api/v1/applications/{name}/sync | Sync syncs an application to its target state
[**application_service_terminate_operation**](ApplicationServiceApi.md#application_service_terminate_operation) | **DELETE** /api/v1/applications/{name}/operation | TerminateOperation terminates the currently running operation
[**application_service_update**](ApplicationServiceApi.md#application_service_update) | **PUT** /api/v1/applications/{application.metadata.name} | Update updates an application
[**application_service_update_spec**](ApplicationServiceApi.md#application_service_update_spec) | **PUT** /api/v1/applications/{name}/spec | UpdateSpec updates an application spec
[**application_service_watch**](ApplicationServiceApi.md#application_service_watch) | **GET** /api/v1/stream/applications | Watch returns stream of application change events
[**application_service_watch_resource_tree**](ApplicationServiceApi.md#application_service_watch_resource_tree) | **GET** /api/v1/stream/applications/{applicationName}/resource-tree | Watch returns stream of application resource tree



## application_service_create

> models::V1alpha1Application application_service_create(body, upsert, validate)
Create creates an application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1Application**](V1alpha1Application.md) |  | [required] |
**upsert** | Option<**bool**> |  |  |
**validate** | Option<**bool**> |  |  |

### Return type

[**models::V1alpha1Application**](v1alpha1Application.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_delete

> serde_json::Value application_service_delete(name, cascade, propagation_policy, app_namespace, project)
Delete deletes an application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**cascade** | Option<**bool**> |  |  |
**propagation_policy** | Option<**String**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_delete_resource

> serde_json::Value application_service_delete_resource(name, namespace, resource_name, version, group, kind, force, orphan, app_namespace, project)
DeleteResource deletes a single application resource

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**namespace** | Option<**String**> |  |  |
**resource_name** | Option<**String**> |  |  |
**version** | Option<**String**> |  |  |
**group** | Option<**String**> |  |  |
**kind** | Option<**String**> |  |  |
**force** | Option<**bool**> |  |  |
**orphan** | Option<**bool**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_get

> models::V1alpha1Application application_service_get(name, refresh, projects, resource_version, selector, repo, app_namespace, project)
Get returns an application by name

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** | the application's name | [required] |
**refresh** | Option<**String**> | forces application reconciliation if set to 'hard'. |  |
**projects** | Option<[**Vec<String>**](String.md)> | the project names to restrict returned list applications. |  |
**resource_version** | Option<**String**> | when specified with a watch call, shows changes that occur after that particular version of a resource. |  |
**selector** | Option<**String**> | the selector to restrict returned list to applications only with matched labels. |  |
**repo** | Option<**String**> | the repoURL to restrict returned list applications. |  |
**app_namespace** | Option<**String**> | the application's namespace. |  |
**project** | Option<[**Vec<String>**](String.md)> | the project names to restrict returned list applications (legacy name for backwards-compatibility). |  |

### Return type

[**models::V1alpha1Application**](v1alpha1Application.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_get_application_sync_windows

> models::ApplicationApplicationSyncWindowsResponse application_service_get_application_sync_windows(name, app_namespace, project)
Get returns sync windows of the application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**models::ApplicationApplicationSyncWindowsResponse**](applicationApplicationSyncWindowsResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_get_manifests

> models::RepositoryManifestResponse application_service_get_manifests(name, revision, app_namespace, project, source_positions, revisions)
GetManifests returns application manifests

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**revision** | Option<**String**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |
**source_positions** | Option<[**Vec<String>**](String.md)> |  |  |
**revisions** | Option<[**Vec<String>**](String.md)> |  |  |

### Return type

[**models::RepositoryManifestResponse**](repositoryManifestResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_get_manifests_with_files

> models::RepositoryManifestResponse application_service_get_manifests_with_files(body)
GetManifestsWithFiles returns application manifests using provided files to generate them

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**ApplicationApplicationManifestQueryWithFilesWrapper**](ApplicationApplicationManifestQueryWithFilesWrapper.md) |  (streaming inputs) | [required] |

### Return type

[**models::RepositoryManifestResponse**](repositoryManifestResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_get_oci_metadata

> models::V1alpha1OciMetadata application_service_get_oci_metadata(name, revision, app_namespace, project, source_index, version_id)
Get the chart metadata (description, maintainers, home) for a specific revision of the application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** | the application's name | [required] |
**revision** | **String** | the revision of the app | [required] |
**app_namespace** | Option<**String**> | the application's namespace. |  |
**project** | Option<**String**> |  |  |
**source_index** | Option<**i32**> | source index (for multi source apps). |  |
**version_id** | Option<**i32**> | versionId from historical data (for multi source apps). |  |

### Return type

[**models::V1alpha1OciMetadata**](v1alpha1OCIMetadata.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_get_resource

> models::ApplicationApplicationResourceResponse application_service_get_resource(name, namespace, resource_name, version, group, kind, app_namespace, project)
GetResource returns single application resource

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**namespace** | Option<**String**> |  |  |
**resource_name** | Option<**String**> |  |  |
**version** | Option<**String**> |  |  |
**group** | Option<**String**> |  |  |
**kind** | Option<**String**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**models::ApplicationApplicationResourceResponse**](applicationApplicationResourceResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_list

> models::V1alpha1ApplicationList application_service_list(name, refresh, projects, resource_version, selector, repo, app_namespace, project)
List returns list of applications

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | Option<**String**> | the application's name. |  |
**refresh** | Option<**String**> | forces application reconciliation if set to 'hard'. |  |
**projects** | Option<[**Vec<String>**](String.md)> | the project names to restrict returned list applications. |  |
**resource_version** | Option<**String**> | when specified with a watch call, shows changes that occur after that particular version of a resource. |  |
**selector** | Option<**String**> | the selector to restrict returned list to applications only with matched labels. |  |
**repo** | Option<**String**> | the repoURL to restrict returned list applications. |  |
**app_namespace** | Option<**String**> | the application's namespace. |  |
**project** | Option<[**Vec<String>**](String.md)> | the project names to restrict returned list applications (legacy name for backwards-compatibility). |  |

### Return type

[**models::V1alpha1ApplicationList**](v1alpha1ApplicationList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_list_links

> models::ApplicationLinksResponse application_service_list_links(name, namespace, project)
ListLinks returns the list of all application deep links

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**models::ApplicationLinksResponse**](applicationLinksResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_list_resource_actions

> models::ApplicationResourceActionsListResponse application_service_list_resource_actions(name, namespace, resource_name, version, group, kind, app_namespace, project)
ListResourceActions returns list of resource actions

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**namespace** | Option<**String**> |  |  |
**resource_name** | Option<**String**> |  |  |
**version** | Option<**String**> |  |  |
**group** | Option<**String**> |  |  |
**kind** | Option<**String**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**models::ApplicationResourceActionsListResponse**](applicationResourceActionsListResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_list_resource_events

> models::V1EventList application_service_list_resource_events(name, resource_namespace, resource_name, resource_uid, app_namespace, project)
ListResourceEvents returns a list of event resources

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**resource_namespace** | Option<**String**> |  |  |
**resource_name** | Option<**String**> |  |  |
**resource_uid** | Option<**String**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**models::V1EventList**](v1EventList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_list_resource_links

> models::ApplicationLinksResponse application_service_list_resource_links(name, namespace, resource_name, version, group, kind, app_namespace, project)
ListResourceLinks returns the list of all resource deep links

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**namespace** | Option<**String**> |  |  |
**resource_name** | Option<**String**> |  |  |
**version** | Option<**String**> |  |  |
**group** | Option<**String**> |  |  |
**kind** | Option<**String**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**models::ApplicationLinksResponse**](applicationLinksResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_managed_resources

> models::ApplicationManagedResourcesResponse application_service_managed_resources(application_name, namespace, name, version, group, kind, app_namespace, project)
ManagedResources returns list of managed resources

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**application_name** | **String** |  | [required] |
**namespace** | Option<**String**> |  |  |
**name** | Option<**String**> |  |  |
**version** | Option<**String**> |  |  |
**group** | Option<**String**> |  |  |
**kind** | Option<**String**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**models::ApplicationManagedResourcesResponse**](applicationManagedResourcesResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_patch

> models::V1alpha1Application application_service_patch(body, name)
Patch patch an application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**ApplicationApplicationPatchRequest**](ApplicationApplicationPatchRequest.md) |  | [required] |
**name** | **String** |  | [required] |

### Return type

[**models::V1alpha1Application**](v1alpha1Application.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_patch_resource

> models::ApplicationApplicationResourceResponse application_service_patch_resource(body, name, namespace, resource_name, version, group, kind, patch_type, app_namespace, project)
PatchResource patch single application resource

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | **String** |  | [required] |
**name** | **String** |  | [required] |
**namespace** | Option<**String**> |  |  |
**resource_name** | Option<**String**> |  |  |
**version** | Option<**String**> |  |  |
**group** | Option<**String**> |  |  |
**kind** | Option<**String**> |  |  |
**patch_type** | Option<**String**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**models::ApplicationApplicationResourceResponse**](applicationApplicationResourceResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_pod_logs

> models::StreamResultOfApplicationLogEntry application_service_pod_logs(name, pod_name, namespace, container, since_seconds, since_time_seconds, since_time_nanos, tail_lines, follow, until_time, filter, kind, group, resource_name, previous, app_namespace, project, match_case)
PodLogs returns stream of log entries for the specified pod. Pod

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**pod_name** | **String** |  | [required] |
**namespace** | Option<**String**> |  |  |
**container** | Option<**String**> |  |  |
**since_seconds** | Option<**String**> |  |  |
**since_time_seconds** | Option<**String**> | Represents seconds of UTC time since Unix epoch 1970-01-01T00:00:00Z. Must be from 0001-01-01T00:00:00Z to 9999-12-31T23:59:59Z inclusive. |  |
**since_time_nanos** | Option<**i32**> | Non-negative fractions of a second at nanosecond resolution. Negative second values with fractions must still have non-negative nanos values that count forward in time. Must be from 0 to 999,999,999 inclusive. This field may be limited in precision depending on context. |  |
**tail_lines** | Option<**String**> |  |  |
**follow** | Option<**bool**> |  |  |
**until_time** | Option<**String**> |  |  |
**filter** | Option<**String**> |  |  |
**kind** | Option<**String**> |  |  |
**group** | Option<**String**> |  |  |
**resource_name** | Option<**String**> |  |  |
**previous** | Option<**bool**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |
**match_case** | Option<**bool**> |  |  |

### Return type

[**models::StreamResultOfApplicationLogEntry**](Stream_result_of_applicationLogEntry.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_pod_logs2

> models::StreamResultOfApplicationLogEntry application_service_pod_logs2(name, namespace, pod_name, container, since_seconds, since_time_seconds, since_time_nanos, tail_lines, follow, until_time, filter, kind, group, resource_name, previous, app_namespace, project, match_case)
PodLogs returns stream of log entries for the specified pod. Pod

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**namespace** | Option<**String**> |  |  |
**pod_name** | Option<**String**> |  |  |
**container** | Option<**String**> |  |  |
**since_seconds** | Option<**String**> |  |  |
**since_time_seconds** | Option<**String**> | Represents seconds of UTC time since Unix epoch 1970-01-01T00:00:00Z. Must be from 0001-01-01T00:00:00Z to 9999-12-31T23:59:59Z inclusive. |  |
**since_time_nanos** | Option<**i32**> | Non-negative fractions of a second at nanosecond resolution. Negative second values with fractions must still have non-negative nanos values that count forward in time. Must be from 0 to 999,999,999 inclusive. This field may be limited in precision depending on context. |  |
**tail_lines** | Option<**String**> |  |  |
**follow** | Option<**bool**> |  |  |
**until_time** | Option<**String**> |  |  |
**filter** | Option<**String**> |  |  |
**kind** | Option<**String**> |  |  |
**group** | Option<**String**> |  |  |
**resource_name** | Option<**String**> |  |  |
**previous** | Option<**bool**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |
**match_case** | Option<**bool**> |  |  |

### Return type

[**models::StreamResultOfApplicationLogEntry**](Stream_result_of_applicationLogEntry.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_resource_tree

> models::V1alpha1ApplicationTree application_service_resource_tree(application_name, namespace, name, version, group, kind, app_namespace, project)
ResourceTree returns resource tree

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**application_name** | **String** |  | [required] |
**namespace** | Option<**String**> |  |  |
**name** | Option<**String**> |  |  |
**version** | Option<**String**> |  |  |
**group** | Option<**String**> |  |  |
**kind** | Option<**String**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**models::V1alpha1ApplicationTree**](v1alpha1ApplicationTree.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_revision_chart_details

> models::V1alpha1ChartDetails application_service_revision_chart_details(name, revision, app_namespace, project, source_index, version_id)
Get the chart metadata (description, maintainers, home) for a specific revision of the application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** | the application's name | [required] |
**revision** | **String** | the revision of the app | [required] |
**app_namespace** | Option<**String**> | the application's namespace. |  |
**project** | Option<**String**> |  |  |
**source_index** | Option<**i32**> | source index (for multi source apps). |  |
**version_id** | Option<**i32**> | versionId from historical data (for multi source apps). |  |

### Return type

[**models::V1alpha1ChartDetails**](v1alpha1ChartDetails.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_revision_metadata

> models::V1alpha1RevisionMetadata application_service_revision_metadata(name, revision, app_namespace, project, source_index, version_id)
Get the meta-data (author, date, tags, message) for a specific revision of the application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** | the application's name | [required] |
**revision** | **String** | the revision of the app | [required] |
**app_namespace** | Option<**String**> | the application's namespace. |  |
**project** | Option<**String**> |  |  |
**source_index** | Option<**i32**> | source index (for multi source apps). |  |
**version_id** | Option<**i32**> | versionId from historical data (for multi source apps). |  |

### Return type

[**models::V1alpha1RevisionMetadata**](v1alpha1RevisionMetadata.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_rollback

> models::V1alpha1Application application_service_rollback(body, name)
Rollback syncs an application to its target state

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**ApplicationApplicationRollbackRequest**](ApplicationApplicationRollbackRequest.md) |  | [required] |
**name** | **String** |  | [required] |

### Return type

[**models::V1alpha1Application**](v1alpha1Application.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_run_resource_action

> serde_json::Value application_service_run_resource_action(body, name, namespace, resource_name, version, group, kind, app_namespace, project)
RunResourceAction runs a resource action

Deprecated: use RunResourceActionV2 instead. This version does not support resource action parameters but is maintained for backward compatibility. It will be removed in a future release.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | **String** |  | [required] |
**name** | **String** |  | [required] |
**namespace** | Option<**String**> |  |  |
**resource_name** | Option<**String**> |  |  |
**version** | Option<**String**> |  |  |
**group** | Option<**String**> |  |  |
**kind** | Option<**String**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_run_resource_action_v2

> serde_json::Value application_service_run_resource_action_v2(body, name)
RunResourceActionV2 runs a resource action with parameters

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**ApplicationResourceActionRunRequestV2**](ApplicationResourceActionRunRequestV2.md) |  | [required] |
**name** | **String** |  | [required] |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_sync

> models::V1alpha1Application application_service_sync(body, name)
Sync syncs an application to its target state

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**ApplicationApplicationSyncRequest**](ApplicationApplicationSyncRequest.md) |  | [required] |
**name** | **String** |  | [required] |

### Return type

[**models::V1alpha1Application**](v1alpha1Application.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_terminate_operation

> serde_json::Value application_service_terminate_operation(name, app_namespace, project)
TerminateOperation terminates the currently running operation

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | **String** |  | [required] |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_update

> models::V1alpha1Application application_service_update(body, application_metadata_name, validate, project)
Update updates an application

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1Application**](V1alpha1Application.md) |  | [required] |
**application_metadata_name** | **String** | Name must be unique within a namespace. Is required when creating resources, although some resources may allow a client to request the generation of an appropriate name automatically. Name is primarily intended for creation idempotence and configuration definition. Cannot be updated. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names#names +optional | [required] |
**validate** | Option<**bool**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**models::V1alpha1Application**](v1alpha1Application.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_update_spec

> models::V1alpha1ApplicationSpec application_service_update_spec(body, name, validate, app_namespace, project)
UpdateSpec updates an application spec

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1ApplicationSpec**](V1alpha1ApplicationSpec.md) |  | [required] |
**name** | **String** |  | [required] |
**validate** | Option<**bool**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**models::V1alpha1ApplicationSpec**](v1alpha1ApplicationSpec.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_watch

> models::StreamResultOfV1alpha1ApplicationWatchEvent application_service_watch(name, refresh, projects, resource_version, selector, repo, app_namespace, project)
Watch returns stream of application change events

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | Option<**String**> | the application's name. |  |
**refresh** | Option<**String**> | forces application reconciliation if set to 'hard'. |  |
**projects** | Option<[**Vec<String>**](String.md)> | the project names to restrict returned list applications. |  |
**resource_version** | Option<**String**> | when specified with a watch call, shows changes that occur after that particular version of a resource. |  |
**selector** | Option<**String**> | the selector to restrict returned list to applications only with matched labels. |  |
**repo** | Option<**String**> | the repoURL to restrict returned list applications. |  |
**app_namespace** | Option<**String**> | the application's namespace. |  |
**project** | Option<[**Vec<String>**](String.md)> | the project names to restrict returned list applications (legacy name for backwards-compatibility). |  |

### Return type

[**models::StreamResultOfV1alpha1ApplicationWatchEvent**](Stream_result_of_v1alpha1ApplicationWatchEvent.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## application_service_watch_resource_tree

> models::StreamResultOfV1alpha1ApplicationTree application_service_watch_resource_tree(application_name, namespace, name, version, group, kind, app_namespace, project)
Watch returns stream of application resource tree

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**application_name** | **String** |  | [required] |
**namespace** | Option<**String**> |  |  |
**name** | Option<**String**> |  |  |
**version** | Option<**String**> |  |  |
**group** | Option<**String**> |  |  |
**kind** | Option<**String**> |  |  |
**app_namespace** | Option<**String**> |  |  |
**project** | Option<**String**> |  |  |

### Return type

[**models::StreamResultOfV1alpha1ApplicationTree**](Stream_result_of_v1alpha1ApplicationTree.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

