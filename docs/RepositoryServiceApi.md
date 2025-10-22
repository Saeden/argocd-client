# \RepositoryServiceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**repository_service_create_repository**](RepositoryServiceApi.md#repository_service_create_repository) | **POST** /api/v1/repositories | CreateRepository creates a new repository configuration
[**repository_service_create_write_repository**](RepositoryServiceApi.md#repository_service_create_write_repository) | **POST** /api/v1/write-repositories | CreateWriteRepository creates a new write repository configuration
[**repository_service_delete_repository**](RepositoryServiceApi.md#repository_service_delete_repository) | **DELETE** /api/v1/repositories/{repo} | DeleteRepository deletes a repository from the configuration
[**repository_service_delete_write_repository**](RepositoryServiceApi.md#repository_service_delete_write_repository) | **DELETE** /api/v1/write-repositories/{repo} | DeleteWriteRepository deletes a write repository from the configuration
[**repository_service_get**](RepositoryServiceApi.md#repository_service_get) | **GET** /api/v1/repositories/{repo} | Get returns a repository or its credentials
[**repository_service_get_app_details**](RepositoryServiceApi.md#repository_service_get_app_details) | **POST** /api/v1/repositories/{source.repoURL}/appdetails | GetAppDetails returns application details by given path
[**repository_service_get_helm_charts**](RepositoryServiceApi.md#repository_service_get_helm_charts) | **GET** /api/v1/repositories/{repo}/helmcharts | GetHelmCharts returns list of helm charts in the specified repository
[**repository_service_get_write**](RepositoryServiceApi.md#repository_service_get_write) | **GET** /api/v1/write-repositories/{repo} | GetWrite returns a repository or its write credentials
[**repository_service_list_apps**](RepositoryServiceApi.md#repository_service_list_apps) | **GET** /api/v1/repositories/{repo}/apps | ListApps returns list of apps in the repo
[**repository_service_list_oci_tags**](RepositoryServiceApi.md#repository_service_list_oci_tags) | **GET** /api/v1/repositories/{repo}/oci-tags | 
[**repository_service_list_refs**](RepositoryServiceApi.md#repository_service_list_refs) | **GET** /api/v1/repositories/{repo}/refs | 
[**repository_service_list_repositories**](RepositoryServiceApi.md#repository_service_list_repositories) | **GET** /api/v1/repositories | ListRepositories gets a list of all configured repositories
[**repository_service_list_write_repositories**](RepositoryServiceApi.md#repository_service_list_write_repositories) | **GET** /api/v1/write-repositories | ListWriteRepositories gets a list of all configured write repositories
[**repository_service_update_repository**](RepositoryServiceApi.md#repository_service_update_repository) | **PUT** /api/v1/repositories/{repo.repo} | UpdateRepository updates a repository configuration
[**repository_service_update_write_repository**](RepositoryServiceApi.md#repository_service_update_write_repository) | **PUT** /api/v1/write-repositories/{repo.repo} | UpdateWriteRepository updates a write repository configuration
[**repository_service_validate_access**](RepositoryServiceApi.md#repository_service_validate_access) | **POST** /api/v1/repositories/{repo}/validate | ValidateAccess validates access to a repository with given parameters
[**repository_service_validate_write_access**](RepositoryServiceApi.md#repository_service_validate_write_access) | **POST** /api/v1/write-repositories/{repo}/validate | ValidateWriteAccess validates write access to a repository with given parameters



## repository_service_create_repository

> models::V1alpha1Repository repository_service_create_repository(body, upsert, creds_only)
CreateRepository creates a new repository configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1Repository**](V1alpha1Repository.md) | Repository definition | [required] |
**upsert** | Option<**bool**> | Whether to create in upsert mode. |  |
**creds_only** | Option<**bool**> | Whether to operate on credential set instead of repository. |  |

### Return type

[**models::V1alpha1Repository**](v1alpha1Repository.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_create_write_repository

> models::V1alpha1Repository repository_service_create_write_repository(body, upsert, creds_only)
CreateWriteRepository creates a new write repository configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1Repository**](V1alpha1Repository.md) | Repository definition | [required] |
**upsert** | Option<**bool**> | Whether to create in upsert mode. |  |
**creds_only** | Option<**bool**> | Whether to operate on credential set instead of repository. |  |

### Return type

[**models::V1alpha1Repository**](v1alpha1Repository.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_delete_repository

> serde_json::Value repository_service_delete_repository(repo, force_refresh, app_project)
DeleteRepository deletes a repository from the configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**repo** | **String** | Repo URL for query | [required] |
**force_refresh** | Option<**bool**> | Whether to force a cache refresh on repo's connection state. |  |
**app_project** | Option<**String**> | App project for query. |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_delete_write_repository

> serde_json::Value repository_service_delete_write_repository(repo, force_refresh, app_project)
DeleteWriteRepository deletes a write repository from the configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**repo** | **String** | Repo URL for query | [required] |
**force_refresh** | Option<**bool**> | Whether to force a cache refresh on repo's connection state. |  |
**app_project** | Option<**String**> | App project for query. |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_get

> models::V1alpha1Repository repository_service_get(repo, force_refresh, app_project)
Get returns a repository or its credentials

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**repo** | **String** | Repo URL for query | [required] |
**force_refresh** | Option<**bool**> | Whether to force a cache refresh on repo's connection state. |  |
**app_project** | Option<**String**> | App project for query. |  |

### Return type

[**models::V1alpha1Repository**](v1alpha1Repository.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_get_app_details

> models::RepositoryRepoAppDetailsResponse repository_service_get_app_details(body, source_repo_url)
GetAppDetails returns application details by given path

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**RepositoryRepoAppDetailsQuery**](RepositoryRepoAppDetailsQuery.md) |  | [required] |
**source_repo_url** | **String** | RepoURL is the URL to the repository (Git or Helm) that contains the application manifests | [required] |

### Return type

[**models::RepositoryRepoAppDetailsResponse**](repositoryRepoAppDetailsResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_get_helm_charts

> models::RepositoryHelmChartsResponse repository_service_get_helm_charts(repo, force_refresh, app_project)
GetHelmCharts returns list of helm charts in the specified repository

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**repo** | **String** | Repo URL for query | [required] |
**force_refresh** | Option<**bool**> | Whether to force a cache refresh on repo's connection state. |  |
**app_project** | Option<**String**> | App project for query. |  |

### Return type

[**models::RepositoryHelmChartsResponse**](repositoryHelmChartsResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_get_write

> models::V1alpha1Repository repository_service_get_write(repo, force_refresh, app_project)
GetWrite returns a repository or its write credentials

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**repo** | **String** | Repo URL for query | [required] |
**force_refresh** | Option<**bool**> | Whether to force a cache refresh on repo's connection state. |  |
**app_project** | Option<**String**> | App project for query. |  |

### Return type

[**models::V1alpha1Repository**](v1alpha1Repository.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_list_apps

> models::RepositoryRepoAppsResponse repository_service_list_apps(repo, revision, app_name, app_project)
ListApps returns list of apps in the repo

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**repo** | **String** |  | [required] |
**revision** | Option<**String**> |  |  |
**app_name** | Option<**String**> |  |  |
**app_project** | Option<**String**> |  |  |

### Return type

[**models::RepositoryRepoAppsResponse**](repositoryRepoAppsResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_list_oci_tags

> models::RepositoryRefs repository_service_list_oci_tags(repo, force_refresh, app_project)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**repo** | **String** | Repo URL for query | [required] |
**force_refresh** | Option<**bool**> | Whether to force a cache refresh on repo's connection state. |  |
**app_project** | Option<**String**> | App project for query. |  |

### Return type

[**models::RepositoryRefs**](repositoryRefs.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_list_refs

> models::RepositoryRefs repository_service_list_refs(repo, force_refresh, app_project)


### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**repo** | **String** | Repo URL for query | [required] |
**force_refresh** | Option<**bool**> | Whether to force a cache refresh on repo's connection state. |  |
**app_project** | Option<**String**> | App project for query. |  |

### Return type

[**models::RepositoryRefs**](repositoryRefs.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_list_repositories

> models::V1alpha1RepositoryList repository_service_list_repositories(repo, force_refresh, app_project)
ListRepositories gets a list of all configured repositories

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**repo** | Option<**String**> | Repo URL for query. |  |
**force_refresh** | Option<**bool**> | Whether to force a cache refresh on repo's connection state. |  |
**app_project** | Option<**String**> | App project for query. |  |

### Return type

[**models::V1alpha1RepositoryList**](v1alpha1RepositoryList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_list_write_repositories

> models::V1alpha1RepositoryList repository_service_list_write_repositories(repo, force_refresh, app_project)
ListWriteRepositories gets a list of all configured write repositories

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**repo** | Option<**String**> | Repo URL for query. |  |
**force_refresh** | Option<**bool**> | Whether to force a cache refresh on repo's connection state. |  |
**app_project** | Option<**String**> | App project for query. |  |

### Return type

[**models::V1alpha1RepositoryList**](v1alpha1RepositoryList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_update_repository

> models::V1alpha1Repository repository_service_update_repository(body, repo_repo)
UpdateRepository updates a repository configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1Repository**](V1alpha1Repository.md) |  | [required] |
**repo_repo** | **String** | Repo contains the URL to the remote repository | [required] |

### Return type

[**models::V1alpha1Repository**](v1alpha1Repository.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_update_write_repository

> models::V1alpha1Repository repository_service_update_write_repository(body, repo_repo)
UpdateWriteRepository updates a write repository configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1Repository**](V1alpha1Repository.md) |  | [required] |
**repo_repo** | **String** | Repo contains the URL to the remote repository | [required] |

### Return type

[**models::V1alpha1Repository**](v1alpha1Repository.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_validate_access

> serde_json::Value repository_service_validate_access(body, repo, username, password, ssh_private_key, insecure, tls_client_cert_data, tls_client_cert_key, r#type, name, enable_oci, github_app_private_key, github_app_id, github_app_installation_id, github_app_enterprise_base_url, proxy, project, gcp_service_account_key, force_http_basic_auth, use_azure_workload_identity, bearer_token, insecure_oci_force_http)
ValidateAccess validates access to a repository with given parameters

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | **String** | The URL to the repo | [required] |
**repo** | **String** | The URL to the repo | [required] |
**username** | Option<**String**> | Username for accessing repo. |  |
**password** | Option<**String**> | Password for accessing repo. |  |
**ssh_private_key** | Option<**String**> | Private key data for accessing SSH repository. |  |
**insecure** | Option<**bool**> | Whether to skip certificate or host key validation. |  |
**tls_client_cert_data** | Option<**String**> | TLS client cert data for accessing HTTPS repository. |  |
**tls_client_cert_key** | Option<**String**> | TLS client cert key for accessing HTTPS repository. |  |
**r#type** | Option<**String**> | The type of the repo. |  |
**name** | Option<**String**> | The name of the repo. |  |
**enable_oci** | Option<**bool**> | Whether helm-oci support should be enabled for this repo. |  |
**github_app_private_key** | Option<**String**> | Github App Private Key PEM data. |  |
**github_app_id** | Option<**String**> | Github App ID of the app used to access the repo. |  |
**github_app_installation_id** | Option<**String**> | Github App Installation ID of the installed GitHub App. |  |
**github_app_enterprise_base_url** | Option<**String**> | Github App Enterprise base url if empty will default to https://api.github.com. |  |
**proxy** | Option<**String**> | HTTP/HTTPS proxy to access the repository. |  |
**project** | Option<**String**> | Reference between project and repository that allow you automatically to be added as item inside SourceRepos project entity. |  |
**gcp_service_account_key** | Option<**String**> | Google Cloud Platform service account key. |  |
**force_http_basic_auth** | Option<**bool**> | Whether to force HTTP basic auth. |  |
**use_azure_workload_identity** | Option<**bool**> | Whether to use azure workload identity for authentication. |  |
**bearer_token** | Option<**String**> | BearerToken contains the bearer token used for Git auth at the repo server. |  |
**insecure_oci_force_http** | Option<**bool**> | Whether https should be disabled for an OCI repo. |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repository_service_validate_write_access

> serde_json::Value repository_service_validate_write_access(body, repo, username, password, ssh_private_key, insecure, tls_client_cert_data, tls_client_cert_key, r#type, name, enable_oci, github_app_private_key, github_app_id, github_app_installation_id, github_app_enterprise_base_url, proxy, project, gcp_service_account_key, force_http_basic_auth, use_azure_workload_identity, bearer_token, insecure_oci_force_http)
ValidateWriteAccess validates write access to a repository with given parameters

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | **String** | The URL to the repo | [required] |
**repo** | **String** | The URL to the repo | [required] |
**username** | Option<**String**> | Username for accessing repo. |  |
**password** | Option<**String**> | Password for accessing repo. |  |
**ssh_private_key** | Option<**String**> | Private key data for accessing SSH repository. |  |
**insecure** | Option<**bool**> | Whether to skip certificate or host key validation. |  |
**tls_client_cert_data** | Option<**String**> | TLS client cert data for accessing HTTPS repository. |  |
**tls_client_cert_key** | Option<**String**> | TLS client cert key for accessing HTTPS repository. |  |
**r#type** | Option<**String**> | The type of the repo. |  |
**name** | Option<**String**> | The name of the repo. |  |
**enable_oci** | Option<**bool**> | Whether helm-oci support should be enabled for this repo. |  |
**github_app_private_key** | Option<**String**> | Github App Private Key PEM data. |  |
**github_app_id** | Option<**String**> | Github App ID of the app used to access the repo. |  |
**github_app_installation_id** | Option<**String**> | Github App Installation ID of the installed GitHub App. |  |
**github_app_enterprise_base_url** | Option<**String**> | Github App Enterprise base url if empty will default to https://api.github.com. |  |
**proxy** | Option<**String**> | HTTP/HTTPS proxy to access the repository. |  |
**project** | Option<**String**> | Reference between project and repository that allow you automatically to be added as item inside SourceRepos project entity. |  |
**gcp_service_account_key** | Option<**String**> | Google Cloud Platform service account key. |  |
**force_http_basic_auth** | Option<**bool**> | Whether to force HTTP basic auth. |  |
**use_azure_workload_identity** | Option<**bool**> | Whether to use azure workload identity for authentication. |  |
**bearer_token** | Option<**String**> | BearerToken contains the bearer token used for Git auth at the repo server. |  |
**insecure_oci_force_http** | Option<**bool**> | Whether https should be disabled for an OCI repo. |  |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

