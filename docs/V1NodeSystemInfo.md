# V1NodeSystemInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**architecture** | Option<**String**> |  | [optional]
**boot_id** | Option<**String**> | Boot ID reported by the node. | [optional]
**container_runtime_version** | Option<**String**> | ContainerRuntime Version reported by the node through runtime remote API (e.g. containerd://1.4.2). | [optional]
**kernel_version** | Option<**String**> | Kernel Version reported by the node from 'uname -r' (e.g. 3.16.0-0.bpo.4-amd64). | [optional]
**kube_proxy_version** | Option<**String**> | Deprecated: KubeProxy Version reported by the node. | [optional]
**kubelet_version** | Option<**String**> | Kubelet Version reported by the node. | [optional]
**machine_id** | Option<**String**> |  | [optional]
**operating_system** | Option<**String**> |  | [optional]
**os_image** | Option<**String**> | OS Image reported by the node from /etc/os-release (e.g. Debian GNU/Linux 7 (wheezy)). | [optional]
**swap** | Option<[**models::V1NodeSwapStatus**](v1NodeSwapStatus.md)> |  | [optional]
**system_uuid** | Option<**String**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


