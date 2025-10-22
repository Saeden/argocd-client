# V1alpha1ResourceOverride

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**actions** | Option<**String**> | Actions defines the set of actions that can be performed on the resource, as a Lua script. | [optional]
**health_lua** | Option<**String**> | HealthLua contains a Lua script that defines custom health checks for the resource. | [optional]
**ignore_differences** | Option<[**models::V1alpha1OverrideIgnoreDiff**](v1alpha1OverrideIgnoreDiff.md)> |  | [optional]
**ignore_resource_updates** | Option<[**models::V1alpha1OverrideIgnoreDiff**](v1alpha1OverrideIgnoreDiff.md)> |  | [optional]
**known_type_fields** | Option<[**Vec<models::V1alpha1KnownTypeField>**](v1alpha1KnownTypeField.md)> | KnownTypeFields lists fields for which unit conversions should be applied. | [optional]
**use_open_libs** | Option<**bool**> | UseOpenLibs indicates whether to use open-source libraries for the resource. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


