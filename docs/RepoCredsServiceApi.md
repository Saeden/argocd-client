# \RepoCredsServiceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**repo_creds_service_create_repository_credentials**](RepoCredsServiceApi.md#repo_creds_service_create_repository_credentials) | **POST** /api/v1/repocreds | CreateRepositoryCredentials creates a new repository credential set
[**repo_creds_service_create_write_repository_credentials**](RepoCredsServiceApi.md#repo_creds_service_create_write_repository_credentials) | **POST** /api/v1/write-repocreds | CreateWriteRepositoryCredentials creates a new repository credential set with write access
[**repo_creds_service_delete_repository_credentials**](RepoCredsServiceApi.md#repo_creds_service_delete_repository_credentials) | **DELETE** /api/v1/repocreds/{url} | DeleteRepositoryCredentials deletes a repository credential set from the configuration
[**repo_creds_service_delete_write_repository_credentials**](RepoCredsServiceApi.md#repo_creds_service_delete_write_repository_credentials) | **DELETE** /api/v1/write-repocreds/{url} | DeleteWriteRepositoryCredentials deletes a repository credential set with write access from the configuration
[**repo_creds_service_list_repository_credentials**](RepoCredsServiceApi.md#repo_creds_service_list_repository_credentials) | **GET** /api/v1/repocreds | ListRepositoryCredentials gets a list of all configured repository credential sets
[**repo_creds_service_list_write_repository_credentials**](RepoCredsServiceApi.md#repo_creds_service_list_write_repository_credentials) | **GET** /api/v1/write-repocreds | ListWriteRepositoryCredentials gets a list of all configured repository credential sets that have write access
[**repo_creds_service_update_repository_credentials**](RepoCredsServiceApi.md#repo_creds_service_update_repository_credentials) | **PUT** /api/v1/repocreds/{creds.url} | UpdateRepositoryCredentials updates a repository credential set
[**repo_creds_service_update_write_repository_credentials**](RepoCredsServiceApi.md#repo_creds_service_update_write_repository_credentials) | **PUT** /api/v1/write-repocreds/{creds.url} | UpdateWriteRepositoryCredentials updates a repository credential set with write access



## repo_creds_service_create_repository_credentials

> models::V1alpha1RepoCreds repo_creds_service_create_repository_credentials(body, upsert)
CreateRepositoryCredentials creates a new repository credential set

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1RepoCreds**](V1alpha1RepoCreds.md) | Repository definition | [required] |
**upsert** | Option<**bool**> | Whether to create in upsert mode. |  |

### Return type

[**models::V1alpha1RepoCreds**](v1alpha1RepoCreds.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repo_creds_service_create_write_repository_credentials

> models::V1alpha1RepoCreds repo_creds_service_create_write_repository_credentials(body, upsert)
CreateWriteRepositoryCredentials creates a new repository credential set with write access

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1RepoCreds**](V1alpha1RepoCreds.md) | Repository definition | [required] |
**upsert** | Option<**bool**> | Whether to create in upsert mode. |  |

### Return type

[**models::V1alpha1RepoCreds**](v1alpha1RepoCreds.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repo_creds_service_delete_repository_credentials

> serde_json::Value repo_creds_service_delete_repository_credentials(url)
DeleteRepositoryCredentials deletes a repository credential set from the configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**url** | **String** |  | [required] |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repo_creds_service_delete_write_repository_credentials

> serde_json::Value repo_creds_service_delete_write_repository_credentials(url)
DeleteWriteRepositoryCredentials deletes a repository credential set with write access from the configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**url** | **String** |  | [required] |

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repo_creds_service_list_repository_credentials

> models::V1alpha1RepoCredsList repo_creds_service_list_repository_credentials(url)
ListRepositoryCredentials gets a list of all configured repository credential sets

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**url** | Option<**String**> | Repo URL for query. |  |

### Return type

[**models::V1alpha1RepoCredsList**](v1alpha1RepoCredsList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repo_creds_service_list_write_repository_credentials

> models::V1alpha1RepoCredsList repo_creds_service_list_write_repository_credentials(url)
ListWriteRepositoryCredentials gets a list of all configured repository credential sets that have write access

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**url** | Option<**String**> | Repo URL for query. |  |

### Return type

[**models::V1alpha1RepoCredsList**](v1alpha1RepoCredsList.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repo_creds_service_update_repository_credentials

> models::V1alpha1RepoCreds repo_creds_service_update_repository_credentials(body, creds_url)
UpdateRepositoryCredentials updates a repository credential set

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1RepoCreds**](V1alpha1RepoCreds.md) |  | [required] |
**creds_url** | **String** | URL is the URL to which these credentials match | [required] |

### Return type

[**models::V1alpha1RepoCreds**](v1alpha1RepoCreds.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## repo_creds_service_update_write_repository_credentials

> models::V1alpha1RepoCreds repo_creds_service_update_write_repository_credentials(body, creds_url)
UpdateWriteRepositoryCredentials updates a repository credential set with write access

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**body** | [**V1alpha1RepoCreds**](V1alpha1RepoCreds.md) |  | [required] |
**creds_url** | **String** | URL is the URL to which these credentials match | [required] |

### Return type

[**models::V1alpha1RepoCreds**](v1alpha1RepoCreds.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

