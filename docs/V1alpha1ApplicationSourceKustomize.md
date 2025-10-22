# V1alpha1ApplicationSourceKustomize

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api_versions** | Option<**Vec<String>**> | APIVersions specifies the Kubernetes resource API versions to pass to Helm when templating manifests. By default, Argo CD uses the API versions of the target cluster. The format is [group/]version/kind. | [optional]
**common_annotations** | Option<**std::collections::HashMap<String, String>**> |  | [optional]
**common_annotations_envsubst** | Option<**bool**> |  | [optional]
**common_labels** | Option<**std::collections::HashMap<String, String>**> |  | [optional]
**components** | Option<**Vec<String>**> |  | [optional]
**force_common_annotations** | Option<**bool**> |  | [optional]
**force_common_labels** | Option<**bool**> |  | [optional]
**ignore_missing_components** | Option<**bool**> |  | [optional]
**images** | Option<**Vec<String>**> |  | [optional]
**kube_version** | Option<**String**> | KubeVersion specifies the Kubernetes API version to pass to Helm when templating manifests. By default, Argo CD uses the Kubernetes version of the target cluster. | [optional]
**label_include_templates** | Option<**bool**> |  | [optional]
**label_without_selector** | Option<**bool**> |  | [optional]
**name_prefix** | Option<**String**> |  | [optional]
**name_suffix** | Option<**String**> |  | [optional]
**namespace** | Option<**String**> |  | [optional]
**patches** | Option<[**Vec<models::V1alpha1KustomizePatch>**](v1alpha1KustomizePatch.md)> |  | [optional]
**replicas** | Option<[**Vec<models::V1alpha1KustomizeReplica>**](v1alpha1KustomizeReplica.md)> |  | [optional]
**version** | Option<**String**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


