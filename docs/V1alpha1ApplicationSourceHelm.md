# V1alpha1ApplicationSourceHelm

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_versions** | Option<**Vec<String>**> | APIVersions specifies the Kubernetes resource API versions to pass to Helm when templating manifests. By default, Argo CD uses the API versions of the target cluster. The format is [group/]version/kind. | [optional]
**file_parameters** | Option<[**Vec<models::V1alpha1HelmFileParameter>**](v1alpha1HelmFileParameter.md)> |  | [optional]
**ignore_missing_value_files** | Option<**bool**> |  | [optional]
**kube_version** | Option<**String**> | KubeVersion specifies the Kubernetes API version to pass to Helm when templating manifests. By default, Argo CD uses the Kubernetes version of the target cluster. | [optional]
**namespace** | Option<**String**> | Namespace is an optional namespace to template with. If left empty, defaults to the app's destination namespace. | [optional]
**parameters** | Option<[**Vec<models::V1alpha1HelmParameter>**](v1alpha1HelmParameter.md)> |  | [optional]
**pass_credentials** | Option<**bool**> |  | [optional]
**release_name** | Option<**String**> |  | [optional]
**skip_crds** | Option<**bool**> |  | [optional]
**skip_schema_validation** | Option<**bool**> |  | [optional]
**skip_tests** | Option<**bool**> | SkipTests skips test manifest installation step (Helm's --skip-tests). | [optional]
**value_files** | Option<**Vec<String>**> |  | [optional]
**values** | Option<**String**> |  | [optional]
**values_object** | Option<[**models::RuntimeRawExtension**](runtimeRawExtension.md)> |  | [optional]
**version** | Option<**String**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


