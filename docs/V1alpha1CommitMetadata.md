# V1alpha1CommitMetadata

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**author** | Option<**String**> | Author is the author of the commit, i.e. `git show -s --format=%an <%ae>`. Must be formatted according to RFC 5322 (mail.Address.String()). Comes from the Argocd-reference-commit-author trailer. | [optional]
**body** | Option<**String**> | Body is the commit message body minus the subject line, i.e. `git show -s --format=%b`. Comes from the Argocd-reference-commit-body trailer. | [optional]
**date** | Option<**String**> | Date is the date of the commit, formatted as by `git show -s --format=%aI` (RFC 3339). It can also be an empty string if the date is unknown. Comes from the Argocd-reference-commit-date trailer. | [optional]
**repo_url** | Option<**String**> | RepoURL is the URL of the repository where the commit is located. Comes from the Argocd-reference-commit-repourl trailer. This value is not validated and should not be used to construct UI links unless it is properly validated and/or sanitized first. | [optional]
**sha** | Option<**String**> | SHA is the commit hash. Comes from the Argocd-reference-commit-sha trailer. | [optional]
**subject** | Option<**String**> | Subject is the commit message subject line, i.e. `git show -s --format=%s`. Comes from the Argocd-reference-commit-subject trailer. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


