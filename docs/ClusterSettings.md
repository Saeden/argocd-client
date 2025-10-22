# ClusterSettings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**additional_urls** | Option<**Vec<String>**> |  | [optional]
**app_label_key** | Option<**String**> |  | [optional]
**apps_in_any_namespace_enabled** | Option<**bool**> |  | [optional]
**config_management_plugins** | Option<[**Vec<models::V1alpha1ConfigManagementPlugin>**](v1alpha1ConfigManagementPlugin.md)> | Deprecated: use sidecar plugins instead. | [optional]
**controller_namespace** | Option<**String**> |  | [optional]
**dex_config** | Option<[**models::ClusterDexConfig**](clusterDexConfig.md)> |  | [optional]
**exec_enabled** | Option<**bool**> |  | [optional]
**google_analytics** | Option<[**models::ClusterGoogleAnalyticsConfig**](clusterGoogleAnalyticsConfig.md)> |  | [optional]
**help** | Option<[**models::ClusterHelp**](clusterHelp.md)> |  | [optional]
**hydrator_enabled** | Option<**bool**> |  | [optional]
**impersonation_enabled** | Option<**bool**> |  | [optional]
**installation_id** | Option<**String**> |  | [optional]
**kustomize_options** | Option<[**models::V1alpha1KustomizeOptions**](v1alpha1KustomizeOptions.md)> |  | [optional]
**kustomize_versions** | Option<**Vec<String>**> |  | [optional]
**oidc_config** | Option<[**models::ClusterOidcConfig**](clusterOIDCConfig.md)> |  | [optional]
**password_pattern** | Option<**String**> |  | [optional]
**plugins** | Option<[**Vec<models::ClusterPlugin>**](clusterPlugin.md)> |  | [optional]
**resource_overrides** | Option<[**std::collections::HashMap<String, models::V1alpha1ResourceOverride>**](v1alpha1ResourceOverride.md)> |  | [optional]
**status_badge_enabled** | Option<**bool**> |  | [optional]
**status_badge_root_url** | Option<**String**> |  | [optional]
**tracking_method** | Option<**String**> |  | [optional]
**ui_banner_content** | Option<**String**> |  | [optional]
**ui_banner_permanent** | Option<**bool**> |  | [optional]
**ui_banner_position** | Option<**String**> |  | [optional]
**ui_banner_url** | Option<**String**> |  | [optional]
**ui_css_url** | Option<**String**> |  | [optional]
**url** | Option<**String**> |  | [optional]
**user_logins_disabled** | Option<**bool**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


