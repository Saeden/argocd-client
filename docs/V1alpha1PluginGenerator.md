# V1alpha1PluginGenerator

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**config_map_ref** | Option<[**models::V1alpha1PluginConfigMapRef**](v1alpha1PluginConfigMapRef.md)> |  | [optional]
**input** | Option<[**models::V1alpha1PluginInput**](v1alpha1PluginInput.md)> |  | [optional]
**requeue_after_seconds** | Option<**i64**> | RequeueAfterSeconds determines how long the ApplicationSet controller will wait before reconciling the ApplicationSet again. | [optional]
**template** | Option<[**models::V1alpha1ApplicationSetTemplate**](v1alpha1ApplicationSetTemplate.md)> |  | [optional]
**values** | Option<**std::collections::HashMap<String, String>**> | Values contains key/value pairs which are passed directly as parameters to the template. These values will not be sent as parameters to the plugin. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


