# V1alpha1HostInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**labels** | Option<**std::collections::HashMap<String, String>**> | Labels holds the labels attached to the host. | [optional]
**name** | Option<**String**> | Name is the hostname or node name in the Kubernetes cluster. | [optional]
**resources_info** | Option<[**Vec<models::V1alpha1HostResourceInfo>**](v1alpha1HostResourceInfo.md)> | ResourcesInfo provides a list of resource usage details for different resource types on this host. | [optional]
**system_info** | Option<[**models::V1NodeSystemInfo**](v1NodeSystemInfo.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


