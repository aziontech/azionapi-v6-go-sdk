# \DeploymentsReleasesAPI

All URIs are relative to *https://stage-api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ArchiveRelease**](DeploymentsReleasesAPI.md#ArchiveRelease) | **Post** /deployments/{deployment_id}/releases/{release_id}/archive | Archive a Release
[**BuildAndActivateRelease**](DeploymentsReleasesAPI.md#BuildAndActivateRelease) | **Post** /deployments/{deployment_id}/build_and_activate | Create, build and activate a Release
[**BuildRelease**](DeploymentsReleasesAPI.md#BuildRelease) | **Post** /deployments/{deployment_id}/releases/{release_id}/build | Build a Release
[**CancelRelease**](DeploymentsReleasesAPI.md#CancelRelease) | **Post** /deployments/{deployment_id}/releases/{release_id}/cancel | Cancel a Release
[**CreateRelease**](DeploymentsReleasesAPI.md#CreateRelease) | **Post** /deployments/{deployment_id}/releases | Create a Release
[**DeleteRelease**](DeploymentsReleasesAPI.md#DeleteRelease) | **Delete** /deployments/{deployment_id}/releases/{release_id} | Delete a Release
[**ListAccountReleases**](DeploymentsReleasesAPI.md#ListAccountReleases) | **Get** /deployments/releases | List Releases of all Deployments
[**ListReleases**](DeploymentsReleasesAPI.md#ListReleases) | **Get** /deployments/{deployment_id}/releases | List Releases
[**PartialUpdateRelease**](DeploymentsReleasesAPI.md#PartialUpdateRelease) | **Patch** /deployments/{deployment_id}/releases/{release_id} | Partially update a Release
[**PatchAndActivateRelease**](DeploymentsReleasesAPI.md#PatchAndActivateRelease) | **Post** /deployments/{deployment_id}/releases/{release_id}/patch_and_activate | Update and activate a Release
[**PromoteRelease**](DeploymentsReleasesAPI.md#PromoteRelease) | **Post** /deployments/{deployment_id}/releases/{release_id}/promote | Promote a Release
[**RetrieveRelease**](DeploymentsReleasesAPI.md#RetrieveRelease) | **Get** /deployments/{deployment_id}/releases/{release_id} | Retrieve details of a Release
[**UpdateRelease**](DeploymentsReleasesAPI.md#UpdateRelease) | **Put** /deployments/{deployment_id}/releases/{release_id} | Update a Release



## ArchiveRelease

> ReleaseAsyncResponse ArchiveRelease(ctx, deploymentId, releaseId).ArchiveReleaseRequest(archiveReleaseRequest).Execute()

Archive a Release



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
	releaseId := "releaseId_example" // string | A unique value identifying the release.
	archiveReleaseRequest := *openapiclient.NewArchiveReleaseRequest("Reason_example") // ArchiveReleaseRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsReleasesAPI.ArchiveRelease(context.Background(), deploymentId, releaseId).ArchiveReleaseRequest(archiveReleaseRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleasesAPI.ArchiveRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ArchiveRelease`: ReleaseAsyncResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsReleasesAPI.ArchiveRelease`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 
**releaseId** | **string** | A unique value identifying the release. | 

### Other Parameters

Other parameters are passed through a pointer to a apiArchiveReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **archiveReleaseRequest** | [**ArchiveReleaseRequest**](ArchiveReleaseRequest.md) |  | 

### Return type

[**ReleaseAsyncResponse**](ReleaseAsyncResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BuildAndActivateRelease

> ReleaseAsyncResponse BuildAndActivateRelease(ctx, deploymentId).BuildAndActivateRequest(buildAndActivateRequest).Execute()

Create, build and activate a Release



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
	buildAndActivateRequest := *openapiclient.NewBuildAndActivateRequest([]openapiclient.BuildAndActivateRequestResourcesInner{*openapiclient.NewBuildAndActivateRequestResourcesInner(int64(123), "ResourceType_example")}) // BuildAndActivateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsReleasesAPI.BuildAndActivateRelease(context.Background(), deploymentId).BuildAndActivateRequest(buildAndActivateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleasesAPI.BuildAndActivateRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BuildAndActivateRelease`: ReleaseAsyncResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsReleasesAPI.BuildAndActivateRelease`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBuildAndActivateReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **buildAndActivateRequest** | [**BuildAndActivateRequest**](BuildAndActivateRequest.md) |  | 

### Return type

[**ReleaseAsyncResponse**](ReleaseAsyncResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BuildRelease

> ReleaseAsyncResponse BuildRelease(ctx, deploymentId, releaseId).Body(body).Execute()

Build a Release



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
	releaseId := "releaseId_example" // string | A unique value identifying the release.
	body := map[string]interface{}{ ... } // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsReleasesAPI.BuildRelease(context.Background(), deploymentId, releaseId).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleasesAPI.BuildRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BuildRelease`: ReleaseAsyncResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsReleasesAPI.BuildRelease`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 
**releaseId** | **string** | A unique value identifying the release. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBuildReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **body** | **map[string]interface{}** |  | 

### Return type

[**ReleaseAsyncResponse**](ReleaseAsyncResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelRelease

> ReleaseResponse CancelRelease(ctx, deploymentId, releaseId).CancelReleaseRequest(cancelReleaseRequest).Execute()

Cancel a Release



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
	releaseId := "releaseId_example" // string | A unique value identifying the release.
	cancelReleaseRequest := *openapiclient.NewCancelReleaseRequest() // CancelReleaseRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsReleasesAPI.CancelRelease(context.Background(), deploymentId, releaseId).CancelReleaseRequest(cancelReleaseRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleasesAPI.CancelRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelRelease`: ReleaseResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsReleasesAPI.CancelRelease`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 
**releaseId** | **string** | A unique value identifying the release. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **cancelReleaseRequest** | [**CancelReleaseRequest**](CancelReleaseRequest.md) |  | 

### Return type

[**ReleaseResponse**](ReleaseResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateRelease

> ReleaseAsyncResponse CreateRelease(ctx, deploymentId).ReleaseCreateRequest(releaseCreateRequest).Execute()

Create a Release



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
	releaseCreateRequest := *openapiclient.NewReleaseCreateRequest([]openapiclient.ReleaseCreateRequestResourcesInner{*openapiclient.NewReleaseCreateRequestResourcesInner(int64(123), "ResourceType_example", "VersionId_example")}) // ReleaseCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsReleasesAPI.CreateRelease(context.Background(), deploymentId).ReleaseCreateRequest(releaseCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleasesAPI.CreateRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateRelease`: ReleaseAsyncResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsReleasesAPI.CreateRelease`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **releaseCreateRequest** | [**ReleaseCreateRequest**](ReleaseCreateRequest.md) |  | 

### Return type

[**ReleaseAsyncResponse**](ReleaseAsyncResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteRelease

> DeleteRelease(ctx, deploymentId, releaseId).Execute()

Delete a Release



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
	releaseId := "releaseId_example" // string | A unique value identifying the release.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.DeploymentsReleasesAPI.DeleteRelease(context.Background(), deploymentId, releaseId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleasesAPI.DeleteRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 
**releaseId** | **string** | A unique value identifying the release. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

 (empty response body)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListAccountReleases

> PaginatedAccountReleaseList ListAccountReleases(ctx).Deployment(deployment).Fields(fields).LastModifiedGte(lastModifiedGte).LastModifiedLte(lastModifiedLte).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).State(state).TrafficRole(trafficRole).Execute()

List Releases of all Deployments



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
	deployment := []string{"Inner_example"} // []string | Filter by Deployment id (accepts comma-separated values). (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	lastModifiedGte := time.Now() // time.Time | Filter by last modified date (greater than or equal). (optional)
	lastModifiedLte := time.Now() // time.Time | Filter by last modified date (less than or equal). (optional)
	ordering := "ordering_example" // string | Which field to use when ordering the results. (Valid fields: id, created_at, last_modified, state, traffic_role) (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	search := "search_example" // string | A search term to filter results. Searches across the following fields: id, deployment_name. (optional)
	state := []string{"Inner_example"} // []string | Filter by state (accepts comma-separated values). (optional)
	trafficRole := "trafficRole_example" // string | Filter by traffic role. `active` returns the Releases that serve traffic. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsReleasesAPI.ListAccountReleases(context.Background()).Deployment(deployment).Fields(fields).LastModifiedGte(lastModifiedGte).LastModifiedLte(lastModifiedLte).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).State(state).TrafficRole(trafficRole).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleasesAPI.ListAccountReleases``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAccountReleases`: PaginatedAccountReleaseList
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsReleasesAPI.ListAccountReleases`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListAccountReleasesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deployment** | **[]string** | Filter by Deployment id (accepts comma-separated values). | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **lastModifiedGte** | **time.Time** | Filter by last modified date (greater than or equal). | 
 **lastModifiedLte** | **time.Time** | Filter by last modified date (less than or equal). | 
 **ordering** | **string** | Which field to use when ordering the results. (Valid fields: id, created_at, last_modified, state, traffic_role) | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **search** | **string** | A search term to filter results. Searches across the following fields: id, deployment_name. | 
 **state** | **[]string** | Filter by state (accepts comma-separated values). | 
 **trafficRole** | **string** | Filter by traffic role. &#x60;active&#x60; returns the Releases that serve traffic. | 

### Return type

[**PaginatedAccountReleaseList**](PaginatedAccountReleaseList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListReleases

> PaginatedReleaseList ListReleases(ctx, deploymentId).Fields(fields).Ordering(ordering).Page(page).PageSize(pageSize).State(state).TrafficRole(trafficRole).Execute()

List Releases



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
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	ordering := "ordering_example" // string | Which field to use when ordering the results. (Valid fields: id, created_at, last_modified, state, traffic_role) (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	state := []string{"Inner_example"} // []string | Filter by state (accepts comma-separated values). (optional)
	trafficRole := "trafficRole_example" // string | Filter by traffic role. `active` returns the Releases that serve traffic. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsReleasesAPI.ListReleases(context.Background(), deploymentId).Fields(fields).Ordering(ordering).Page(page).PageSize(pageSize).State(state).TrafficRole(trafficRole).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleasesAPI.ListReleases``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListReleases`: PaginatedReleaseList
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsReleasesAPI.ListReleases`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListReleasesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **ordering** | **string** | Which field to use when ordering the results. (Valid fields: id, created_at, last_modified, state, traffic_role) | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **state** | **[]string** | Filter by state (accepts comma-separated values). | 
 **trafficRole** | **string** | Filter by traffic role. &#x60;active&#x60; returns the Releases that serve traffic. | 

### Return type

[**PaginatedReleaseList**](PaginatedReleaseList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateRelease

> ReleaseResponse PartialUpdateRelease(ctx, deploymentId, releaseId).PatchedReleaseRequest(patchedReleaseRequest).Execute()

Partially update a Release



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
	releaseId := "releaseId_example" // string | A unique value identifying the release.
	patchedReleaseRequest := *openapiclient.NewPatchedReleaseRequest() // PatchedReleaseRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsReleasesAPI.PartialUpdateRelease(context.Background(), deploymentId, releaseId).PatchedReleaseRequest(patchedReleaseRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleasesAPI.PartialUpdateRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateRelease`: ReleaseResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsReleasesAPI.PartialUpdateRelease`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 
**releaseId** | **string** | A unique value identifying the release. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **patchedReleaseRequest** | [**PatchedReleaseRequest**](PatchedReleaseRequest.md) |  | 

### Return type

[**ReleaseResponse**](ReleaseResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchAndActivateRelease

> ReleaseAsyncResponse PatchAndActivateRelease(ctx, deploymentId, releaseId).PatchedReleaseRequest(patchedReleaseRequest).Execute()

Update and activate a Release



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
	releaseId := "releaseId_example" // string | A unique value identifying the release.
	patchedReleaseRequest := *openapiclient.NewPatchedReleaseRequest() // PatchedReleaseRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsReleasesAPI.PatchAndActivateRelease(context.Background(), deploymentId, releaseId).PatchedReleaseRequest(patchedReleaseRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleasesAPI.PatchAndActivateRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchAndActivateRelease`: ReleaseAsyncResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsReleasesAPI.PatchAndActivateRelease`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 
**releaseId** | **string** | A unique value identifying the release. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchAndActivateReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **patchedReleaseRequest** | [**PatchedReleaseRequest**](PatchedReleaseRequest.md) |  | 

### Return type

[**ReleaseAsyncResponse**](ReleaseAsyncResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PromoteRelease

> ReleaseAsyncResponse PromoteRelease(ctx, deploymentId, releaseId).PromoteReleaseRequest(promoteReleaseRequest).Execute()

Promote a Release



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
	releaseId := "releaseId_example" // string | A unique value identifying the release.
	promoteReleaseRequest := *openapiclient.NewPromoteReleaseRequest("TargetDeploymentId_example") // PromoteReleaseRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsReleasesAPI.PromoteRelease(context.Background(), deploymentId, releaseId).PromoteReleaseRequest(promoteReleaseRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleasesAPI.PromoteRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PromoteRelease`: ReleaseAsyncResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsReleasesAPI.PromoteRelease`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 
**releaseId** | **string** | A unique value identifying the release. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPromoteReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **promoteReleaseRequest** | [**PromoteReleaseRequest**](PromoteReleaseRequest.md) |  | 

### Return type

[**ReleaseAsyncResponse**](ReleaseAsyncResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveRelease

> ReleaseRetrieveResponse RetrieveRelease(ctx, deploymentId, releaseId).Fields(fields).Execute()

Retrieve details of a Release



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
	releaseId := "releaseId_example" // string | A unique value identifying the release.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsReleasesAPI.RetrieveRelease(context.Background(), deploymentId, releaseId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleasesAPI.RetrieveRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveRelease`: ReleaseRetrieveResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsReleasesAPI.RetrieveRelease`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 
**releaseId** | **string** | A unique value identifying the release. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**ReleaseRetrieveResponse**](ReleaseRetrieveResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateRelease

> ReleaseResponse UpdateRelease(ctx, deploymentId, releaseId).ReleaseRequest(releaseRequest).Execute()

Update a Release



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
	releaseId := "releaseId_example" // string | A unique value identifying the release.
	releaseRequest := *openapiclient.NewReleaseRequest([]openapiclient.ReleaseCreateRequestResourcesInner{*openapiclient.NewReleaseCreateRequestResourcesInner(int64(123), "ResourceType_example", "VersionId_example")}, *openapiclient.NewReleaseOrigin("Type_example", "SourceEnvironmentId_example", "SourceReleaseId_example", "PromotedFrom_example")) // ReleaseRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsReleasesAPI.UpdateRelease(context.Background(), deploymentId, releaseId).ReleaseRequest(releaseRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleasesAPI.UpdateRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateRelease`: ReleaseResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsReleasesAPI.UpdateRelease`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 
**releaseId** | **string** | A unique value identifying the release. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **releaseRequest** | [**ReleaseRequest**](ReleaseRequest.md) |  | 

### Return type

[**ReleaseResponse**](ReleaseResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

