# \DeploymentsVersionsAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CancelDeploymentVersionBuild**](DeploymentsVersionsAPI.md#CancelDeploymentVersionBuild) | **Post** /deployments/{deployment_id}/versions/{version_id}/cancel | Cancel an in-flight deployment version build
[**ListDeploymentVersions**](DeploymentsVersionsAPI.md#ListDeploymentVersions) | **Get** /deployments/{deployment_id}/versions | List deployment versions
[**RetrieveDeploymentVersion**](DeploymentsVersionsAPI.md#RetrieveDeploymentVersion) | **Get** /deployments/{deployment_id}/versions/{version_id} | Retrieve a deployment version
[**RevertDeploymentVersion**](DeploymentsVersionsAPI.md#RevertDeploymentVersion) | **Post** /deployments/{deployment_id}/versions/{version_id}/revert | Revert to a deployment version



## CancelDeploymentVersionBuild

> DeploymentVersionMeta CancelDeploymentVersionBuild(ctx, deploymentId, versionId).DeploymentVersionCancelRequest(deploymentVersionCancelRequest).Execute()

Cancel an in-flight deployment version build



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	deploymentId := "deploymentId_example" // string | A unique value identifying the deployment.
	versionId := "versionId_example" // string | A unique value identifying the version.
	deploymentVersionCancelRequest := *openapiclient.NewDeploymentVersionCancelRequest() // DeploymentVersionCancelRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsVersionsAPI.CancelDeploymentVersionBuild(context.Background(), deploymentId, versionId).DeploymentVersionCancelRequest(deploymentVersionCancelRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsVersionsAPI.CancelDeploymentVersionBuild``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelDeploymentVersionBuild`: DeploymentVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsVersionsAPI.CancelDeploymentVersionBuild`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 
**versionId** | **string** | A unique value identifying the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelDeploymentVersionBuildRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **deploymentVersionCancelRequest** | [**DeploymentVersionCancelRequest**](DeploymentVersionCancelRequest.md) |  | 

### Return type

[**DeploymentVersionMeta**](DeploymentVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDeploymentVersions

> PaginatedDeploymentVersionList ListDeploymentVersions(ctx, deploymentId).CreatedAtGte(createdAtGte).CreatedAtLte(createdAtLte).Description(description).Fields(fields).LastEditor(lastEditor).Ordering(ordering).Page(page).PageSize(pageSize).ReadyAtGte(readyAtGte).ReadyAtLte(readyAtLte).Search(search).Version(version).VersionGte(versionGte).VersionLte(versionLte).VersionState(versionState).VersionStateIn(versionStateIn).Execute()

List deployment versions



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	deploymentId := "deploymentId_example" // string | A unique value identifying the deployment.
	createdAtGte := time.Now() // time.Time | Filter by creation date (greater than or equal). (optional)
	createdAtLte := time.Now() // time.Time | Filter by creation date (less than or equal). (optional)
	description := "description_example" // string | Filter by description (case-insensitive, partial match). (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	lastEditor := "lastEditor_example" // string | Filter by last editor (case-insensitive, partial match). (optional)
	ordering := "ordering_example" // string | Which field to use when ordering the results. (Valid fields: version, version_state, created_at, ready_at, last_editor) (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	readyAtGte := time.Now() // time.Time | Filter by ready date (greater than or equal). (optional)
	readyAtLte := time.Now() // time.Time | Filter by ready date (less than or equal). (optional)
	search := "search_example" // string | A search term. (optional)
	version := int32(56) // int32 | Filter by version. (optional)
	versionGte := int32(56) // int32 | Filter by version (greater than or equal). (optional)
	versionLte := int32(56) // int32 | Filter by version (less than or equal). (optional)
	versionState := []string{"Inner_example"} // []string | Filter by version state (accepts comma-separated values). (optional)
	versionStateIn := []string{"Inner_example"} // []string | Filter by version_state (accepts comma-separated values). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsVersionsAPI.ListDeploymentVersions(context.Background(), deploymentId).CreatedAtGte(createdAtGte).CreatedAtLte(createdAtLte).Description(description).Fields(fields).LastEditor(lastEditor).Ordering(ordering).Page(page).PageSize(pageSize).ReadyAtGte(readyAtGte).ReadyAtLte(readyAtLte).Search(search).Version(version).VersionGte(versionGte).VersionLte(versionLte).VersionState(versionState).VersionStateIn(versionStateIn).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsVersionsAPI.ListDeploymentVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDeploymentVersions`: PaginatedDeploymentVersionList
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsVersionsAPI.ListDeploymentVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListDeploymentVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createdAtGte** | **time.Time** | Filter by creation date (greater than or equal). | 
 **createdAtLte** | **time.Time** | Filter by creation date (less than or equal). | 
 **description** | **string** | Filter by description (case-insensitive, partial match). | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **lastEditor** | **string** | Filter by last editor (case-insensitive, partial match). | 
 **ordering** | **string** | Which field to use when ordering the results. (Valid fields: version, version_state, created_at, ready_at, last_editor) | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **readyAtGte** | **time.Time** | Filter by ready date (greater than or equal). | 
 **readyAtLte** | **time.Time** | Filter by ready date (less than or equal). | 
 **search** | **string** | A search term. | 
 **version** | **int32** | Filter by version. | 
 **versionGte** | **int32** | Filter by version (greater than or equal). | 
 **versionLte** | **int32** | Filter by version (less than or equal). | 
 **versionState** | **[]string** | Filter by version state (accepts comma-separated values). | 
 **versionStateIn** | **[]string** | Filter by version_state (accepts comma-separated values). | 

### Return type

[**PaginatedDeploymentVersionList**](PaginatedDeploymentVersionList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveDeploymentVersion

> DeploymentVersion RetrieveDeploymentVersion(ctx, deploymentId, versionId).Fields(fields).Execute()

Retrieve a deployment version



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	deploymentId := "deploymentId_example" // string | A unique value identifying the deployment.
	versionId := "versionId_example" // string | A unique value identifying the version.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsVersionsAPI.RetrieveDeploymentVersion(context.Background(), deploymentId, versionId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsVersionsAPI.RetrieveDeploymentVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveDeploymentVersion`: DeploymentVersion
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsVersionsAPI.RetrieveDeploymentVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 
**versionId** | **string** | A unique value identifying the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveDeploymentVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**DeploymentVersion**](DeploymentVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RevertDeploymentVersion

> DeploymentVersionMeta RevertDeploymentVersion(ctx, deploymentId, versionId).DeploymentVersionRevertRequest(deploymentVersionRevertRequest).Execute()

Revert to a deployment version



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	deploymentId := "deploymentId_example" // string | A unique value identifying the deployment.
	versionId := "versionId_example" // string | A unique value identifying the version.
	deploymentVersionRevertRequest := *openapiclient.NewDeploymentVersionRevertRequest() // DeploymentVersionRevertRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsVersionsAPI.RevertDeploymentVersion(context.Background(), deploymentId, versionId).DeploymentVersionRevertRequest(deploymentVersionRevertRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsVersionsAPI.RevertDeploymentVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RevertDeploymentVersion`: DeploymentVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsVersionsAPI.RevertDeploymentVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 
**versionId** | **string** | A unique value identifying the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRevertDeploymentVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **deploymentVersionRevertRequest** | [**DeploymentVersionRevertRequest**](DeploymentVersionRevertRequest.md) |  | 

### Return type

[**DeploymentVersionMeta**](DeploymentVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

