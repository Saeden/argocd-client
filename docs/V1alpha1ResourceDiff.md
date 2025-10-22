# V1alpha1ResourceDiff

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**diff** | Option<**String**> | Diff contains the JSON patch representing the difference between the live and target resource. Deprecated: Use NormalizedLiveState and PredictedLiveState instead to compute differences. | [optional]
**group** | Option<**String**> | Group represents the API group of the resource (e.g., \"apps\" for Deployments). | [optional]
**hook** | Option<**bool**> | Hook indicates whether this resource is a hook resource (e.g., pre-sync or post-sync hooks). | [optional]
**kind** | Option<**String**> | Kind represents the Kubernetes resource kind (e.g., \"Deployment\", \"Service\"). | [optional]
**live_state** | Option<**String**> | LiveState contains the JSON-serialized resource manifest of the resource currently running in the cluster. | [optional]
**modified** | Option<**bool**> | Modified indicates whether the live resource has changes compared to the target resource. | [optional]
**name** | Option<**String**> | Name is the name of the resource. | [optional]
**namespace** | Option<**String**> | Namespace specifies the namespace where the resource exists. | [optional]
**normalized_live_state** | Option<**String**> | NormalizedLiveState contains the JSON-serialized live resource state after applying normalizations. Normalizations may include ignoring irrelevant fields like timestamps or defaults applied by Kubernetes. | [optional]
**predicted_live_state** | Option<**String**> | PredictedLiveState contains the JSON-serialized resource state that Argo CD predicts based on the combination of the normalized live state and the desired target state. | [optional]
**resource_version** | Option<**String**> | ResourceVersion is the Kubernetes resource version, which helps in tracking changes. | [optional]
**target_state** | Option<**String**> | TargetState contains the JSON-serialized resource manifest as defined in the Git/Helm repository. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


