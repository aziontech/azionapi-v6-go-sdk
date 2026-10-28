# \DeploymentsReleasesAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ArchiveRelease**](DeploymentsReleasesAPI.md#ArchiveRelease) | **Post** /deployments/{deployment_id}/releases/{release_id}/archive | Archive a release
[**BuildRelease**](DeploymentsReleasesAPI.md#BuildRelease) | **Post** /deployments/{deployment_id}/releases/{release_id}/build | Finalize a draft release (send to edge via outbox)
[**CancelRelease**](DeploymentsReleasesAPI.md#CancelRelease) | **Post** /deployments/{deployment_id}/releases/{release_id}/cancel | Cancel a release
[**CreateRelease**](DeploymentsReleasesAPI.md#CreateRelease) | **Post** /deployments/{deployment_id}/releases | Create a draft release
[**DeleteRelease**](DeploymentsReleasesAPI.md#DeleteRelease) | **Delete** /deployments/{deployment_id}/releases/{release_id} | Delete a release
[**ListAccountReleases**](DeploymentsReleasesAPI.md#ListAccountReleases) | **Get** /deployments/releases | List every release of the account
[**ListReleases**](DeploymentsReleasesAPI.md#ListReleases) | **Get** /deployments/{deployment_id}/releases | List releases
[**PartialUpdateRelease**](DeploymentsReleasesAPI.md#PartialUpdateRelease) | **Patch** /deployments/{deployment_id}/releases/{release_id} | Patch a release
[**PromoteRelease**](DeploymentsReleasesAPI.md#PromoteRelease) | **Post** /deployments/{deployment_id}/releases/{release_id}/promote | Promote a release
[**RetrieveRelease**](DeploymentsReleasesAPI.md#RetrieveRelease) | **Get** /deployments/{deployment_id}/releases/{release_id} | Get a release
[**UpdateRelease**](DeploymentsReleasesAPI.md#UpdateRelease) | **Put** /deployments/{deployment_id}/releases/{release_id} | Replace a release



## ArchiveRelease

> ReleaseAsyncResponse ArchiveRelease(ctx, deploymentId, releaseId).ArchiveReleaseRequest(archiveReleaseRequest).Execute()

Archive a release



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


## BuildRelease

> ReleaseAsyncResponse BuildRelease(ctx, deploymentId, releaseId).Body(body).Execute()

Finalize a draft release (send to edge via outbox)



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
	body := map[string]interface{}{ ... } // map[string]interface{} | 

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

Cancel a release



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

Create a draft release



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
	releaseCreateRequest := *openapiclient.NewReleaseCreateRequest() // ReleaseCreateRequest | 

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

> DeleteResponse DeleteRelease(ctx, deploymentId, releaseId).Execute()

Delete a release



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
	resp, r, err := apiClient.DeploymentsReleasesAPI.DeleteRelease(context.Background(), deploymentId, releaseId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleasesAPI.DeleteRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteRelease`: DeleteResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsReleasesAPI.DeleteRelease`: %v\n", resp)
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

[**DeleteResponse**](DeleteResponse.md)

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

List every release of the account



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
	deployment := []string{"Inner_example"} // []string | Restrict the listing to these deployments. Comma-separated (`deployment=A,B`) or repeated (`deployment=A&deployment=B`). Max 100. An id that does not exist, or belongs to another account, yields an empty page rather than a 404. (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	lastModifiedGte := time.Now() // time.Time | Only releases modified at or after this ISO-8601 timestamp. (optional)
	lastModifiedLte := time.Now() // time.Time | Only releases modified at or before this ISO-8601 timestamp. (optional)
	ordering := "ordering_example" // string | Comma-separated sort fields. Prefix with `-` for descending. Allowed: `id`, `created_at`, `last_modified`, `state`, `traffic_role`. Default: `-last_modified,-id`. (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	search := "search_example" // string | Free-text search. Matches a release short_id by prefix OR the parent deployment name by substring, case-insensitive. LIKE metacharacters are literal. (optional)
	state := []string{"Inner_example"} // []string | Filter by release state. Comma-separated (`state=ready,building`) or repeated (`state=ready&state=building`). (optional)
	trafficRole := "trafficRole_example" // string | Only releases currently serving traffic. The roles this covers are resolved per parent `deployment_policy`: `single_version` → ACTIVE/CANDIDATE, `versioned_urls` → ACTIVE/VALID_URL. Only `active` is accepted. (optional)

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
 **deployment** | **[]string** | Restrict the listing to these deployments. Comma-separated (&#x60;deployment&#x3D;A,B&#x60;) or repeated (&#x60;deployment&#x3D;A&amp;deployment&#x3D;B&#x60;). Max 100. An id that does not exist, or belongs to another account, yields an empty page rather than a 404. | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **lastModifiedGte** | **time.Time** | Only releases modified at or after this ISO-8601 timestamp. | 
 **lastModifiedLte** | **time.Time** | Only releases modified at or before this ISO-8601 timestamp. | 
 **ordering** | **string** | Comma-separated sort fields. Prefix with &#x60;-&#x60; for descending. Allowed: &#x60;id&#x60;, &#x60;created_at&#x60;, &#x60;last_modified&#x60;, &#x60;state&#x60;, &#x60;traffic_role&#x60;. Default: &#x60;-last_modified,-id&#x60;. | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **search** | **string** | Free-text search. Matches a release short_id by prefix OR the parent deployment name by substring, case-insensitive. LIKE metacharacters are literal. | 
 **state** | **[]string** | Filter by release state. Comma-separated (&#x60;state&#x3D;ready,building&#x60;) or repeated (&#x60;state&#x3D;ready&amp;state&#x3D;building&#x60;). | 
 **trafficRole** | **string** | Only releases currently serving traffic. The roles this covers are resolved per parent &#x60;deployment_policy&#x60;: &#x60;single_version&#x60; → ACTIVE/CANDIDATE, &#x60;versioned_urls&#x60; → ACTIVE/VALID_URL. Only &#x60;active&#x60; is accepted. | 

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

List releases



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
	ordering := "ordering_example" // string | Comma-separated sort fields. Prefix with `-` for descending. Allowed: `id`, `created_at`, `last_modified`, `state`, `traffic_role`. Default: `-created_at,-id`. (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	state := []string{"Inner_example"} // []string | Filter by one or more lifecycle states. Pass a comma-separated list (`state=ready,building`) or repeat the key (`state=ready&state=building`). `deleted` is rejected — it is never listed. `deleting` stays listed so a stuck delete can be found. (optional)
	trafficRole := "trafficRole_example" // string | Semantic filter — `active` returns what is currently serving traffic. single_version → ACTIVE+CANDIDATE; versioned_urls → ACTIVE+VALID_URL. (optional)

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
 **ordering** | **string** | Comma-separated sort fields. Prefix with &#x60;-&#x60; for descending. Allowed: &#x60;id&#x60;, &#x60;created_at&#x60;, &#x60;last_modified&#x60;, &#x60;state&#x60;, &#x60;traffic_role&#x60;. Default: &#x60;-created_at,-id&#x60;. | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **state** | **[]string** | Filter by one or more lifecycle states. Pass a comma-separated list (&#x60;state&#x3D;ready,building&#x60;) or repeat the key (&#x60;state&#x3D;ready&amp;state&#x3D;building&#x60;). &#x60;deleted&#x60; is rejected — it is never listed. &#x60;deleting&#x60; stays listed so a stuck delete can be found. | 
 **trafficRole** | **string** | Semantic filter — &#x60;active&#x60; returns what is currently serving traffic. single_version → ACTIVE+CANDIDATE; versioned_urls → ACTIVE+VALID_URL. | 

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

Patch a release



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


## PromoteRelease

> ReleaseAsyncResponse PromoteRelease(ctx, deploymentId, releaseId).PromoteReleaseRequest(promoteReleaseRequest).Execute()

Promote a release



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

Get a release



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

Replace a release



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
	releaseRequest := *openapiclient.NewReleaseRequest([]openapiclient.PatchedReleaseRequestResourcesInner{*openapiclient.NewPatchedReleaseRequestResourcesInner(int64(123), "ResourceType_example", "VersionId_example")}, *openapiclient.NewAccountReleaseOrigin("Type_example", "SourceEnvironmentId_example", "SourceReleaseId_example", "PromotedFrom_example")) // ReleaseRequest | 

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

