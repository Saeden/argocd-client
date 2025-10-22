# V1alpha1ApplicationSource

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**chart** | Option<**String**> | Chart is a Helm chart name, and must be specified for applications sourced from a Helm repo. | [optional]
**directory** | Option<[**models::V1alpha1ApplicationSourceDirectory**](v1alpha1ApplicationSourceDirectory.md)> |  | [optional]
**helm** | Option<[**models::V1alpha1ApplicationSourceHelm**](v1alpha1ApplicationSourceHelm.md)> |  | [optional]
**kustomize** | Option<[**models::V1alpha1ApplicationSourceKustomize**](v1alpha1ApplicationSourceKustomize.md)> |  | [optional]
**name** | Option<**String**> | Name is used to refer to a source and is displayed in the UI. It is used in multi-source Applications. | [optional]
**path** | Option<**String**> | Path is a directory path within the Git repository, and is only valid for applications sourced from Git. | [optional]
**plugin** | Option<[**models::V1alpha1ApplicationSourcePlugin**](v1alpha1ApplicationSourcePlugin.md)> |  | [optional]
**r#ref** | Option<**String**> | Ref is reference to another source within sources field. This field will not be used if used with a `source` tag. | [optional]
**repo_url** | Option<**String**> |  | [optional]
**target_revision** | Option<**String**> | TargetRevision defines the revision of the source to sync the application to. In case of Git, this can be commit, tag, or branch. If omitted, will equal to HEAD. In case of Helm, this is a semver tag for the Chart's version. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


