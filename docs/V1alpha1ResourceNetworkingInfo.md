# V1alpha1ResourceNetworkingInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**external_urls** | Option<**Vec<String>**> | ExternalURLs holds a list of URLs that should be accessible externally. This field is typically populated for Ingress resources based on their hostname rules. | [optional]
**ingress** | Option<[**Vec<models::V1LoadBalancerIngress>**](v1LoadBalancerIngress.md)> | Ingress provides information about external access points (e.g., load balancer ingress) for this resource. | [optional]
**labels** | Option<**std::collections::HashMap<String, String>**> | Labels holds the labels associated with this networking resource. | [optional]
**target_labels** | Option<**std::collections::HashMap<String, String>**> | TargetLabels represents labels associated with the target resources that this resource communicates with. | [optional]
**target_refs** | Option<[**Vec<models::V1alpha1ResourceRef>**](v1alpha1ResourceRef.md)> | TargetRefs contains references to other resources that this resource interacts with, such as Services or Pods. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


