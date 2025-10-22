# V1alpha1PullRequestGenerator

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**azuredevops** | Option<[**models::V1alpha1PullRequestGeneratorAzureDevOps**](v1alpha1PullRequestGeneratorAzureDevOps.md)> |  | [optional]
**bitbucket** | Option<[**models::V1alpha1PullRequestGeneratorBitbucket**](v1alpha1PullRequestGeneratorBitbucket.md)> |  | [optional]
**bitbucket_server** | Option<[**models::V1alpha1PullRequestGeneratorBitbucketServer**](v1alpha1PullRequestGeneratorBitbucketServer.md)> |  | [optional]
**filters** | Option<[**Vec<models::V1alpha1PullRequestGeneratorFilter>**](v1alpha1PullRequestGeneratorFilter.md)> | Filters for which pull requests should be considered. | [optional]
**gitea** | Option<[**models::V1alpha1PullRequestGeneratorGitea**](v1alpha1PullRequestGeneratorGitea.md)> |  | [optional]
**github** | Option<[**models::V1alpha1PullRequestGeneratorGithub**](v1alpha1PullRequestGeneratorGithub.md)> |  | [optional]
**gitlab** | Option<[**models::V1alpha1PullRequestGeneratorGitLab**](v1alpha1PullRequestGeneratorGitLab.md)> |  | [optional]
**requeue_after_seconds** | Option<**i64**> | Standard parameters. | [optional]
**template** | Option<[**models::V1alpha1ApplicationSetTemplate**](v1alpha1ApplicationSetTemplate.md)> |  | [optional]
**values** | Option<**std::collections::HashMap<String, String>**> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


