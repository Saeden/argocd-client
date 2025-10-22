# RepositoryParameterAnnouncement

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**array** | Option<**Vec<String>**> | array is the default value of the parameter if the parameter is an array. | [optional]
**collection_type** | Option<**String**> | collectionType is the type of value this parameter holds - either a single value (a string) or a collection (array or map). If collectionType is set, only the field with that type will be used. If collectionType is not set, `string` is the default. If collectionType is set to an invalid value, a validation error is thrown. | [optional]
**item_type** | Option<**String**> | itemType determines the primitive data type represented by the parameter. Parameters are always encoded as strings, but this field lets them be interpreted as other primitive types. | [optional]
**map** | Option<**std::collections::HashMap<String, String>**> | map is the default value of the parameter if the parameter is a map. | [optional]
**name** | Option<**String**> | name is the name identifying a parameter. | [optional]
**required** | Option<**bool**> | required defines if this given parameter is mandatory. | [optional]
**string** | Option<**String**> | string is the default value of the parameter if the parameter is a string. | [optional]
**title** | Option<**String**> | title is a human-readable text of the parameter name. | [optional]
**tooltip** | Option<**String**> | tooltip is a human-readable description of the parameter. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


