# V1alpha1ScmProviderGenerator

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**aws_code_commit** | Option<[**models::V1alpha1ScmProviderGeneratorAwsCodeCommit**](v1alpha1SCMProviderGeneratorAWSCodeCommit.md)> |  | [optional]
**azure_dev_ops** | Option<[**models::V1alpha1ScmProviderGeneratorAzureDevOps**](v1alpha1SCMProviderGeneratorAzureDevOps.md)> |  | [optional]
**bitbucket** | Option<[**models::V1alpha1ScmProviderGeneratorBitbucket**](v1alpha1SCMProviderGeneratorBitbucket.md)> |  | [optional]
**bitbucket_server** | Option<[**models::V1alpha1ScmProviderGeneratorBitbucketServer**](v1alpha1SCMProviderGeneratorBitbucketServer.md)> |  | [optional]
**clone_protocol** | Option<**String**> | Which protocol to use for the SCM URL. Default is provider-specific but ssh if possible. Not all providers necessarily support all protocols. | [optional]
**filters** | Option<[**Vec<models::V1alpha1ScmProviderGeneratorFilter>**](v1alpha1SCMProviderGeneratorFilter.md)> | Filters for which repos should be considered. | [optional]
**gitea** | Option<[**models::V1alpha1ScmProviderGeneratorGitea**](v1alpha1SCMProviderGeneratorGitea.md)> |  | [optional]
**github** | Option<[**models::V1alpha1ScmProviderGeneratorGithub**](v1alpha1SCMProviderGeneratorGithub.md)> |  | [optional]
**gitlab** | Option<[**models::V1alpha1ScmProviderGeneratorGitlab**](v1alpha1SCMProviderGeneratorGitlab.md)> |  | [optional]
**requeue_after_seconds** | Option<**i64**> | Standard parameters. | [optional]
**template** | Option<[**models::V1alpha1ApplicationSetTemplate**](v1alpha1ApplicationSetTemplate.md)> |  | [optional]
**values** | Option<**std::collections::HashMap<String, String>**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


