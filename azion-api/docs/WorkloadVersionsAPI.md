# \WorkloadVersionsAPI

All URIs are relative to *https://stage-api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListWorkloadVersions**](WorkloadVersionsAPI.md#ListWorkloadVersions) | **Get** /workspace/workloads/{workload_id}/versions | List Workload versions
[**RetrieveWorkloadVersion**](WorkloadVersionsAPI.md#RetrieveWorkloadVersion) | **Get** /workspace/workloads/{workload_id}/versions/{version_id} | Retrieve a Workload version
[**RevertWorkloadVersion**](WorkloadVersionsAPI.md#RevertWorkloadVersion) | **Post** /workspace/workloads/{workload_id}/versions/{version_id}/revert | Revert to a Workload version



## ListWorkloadVersions

> PaginatedWorkloadVersionList ListWorkloadVersions(ctx, workloadId).Page(page).PageSize(pageSize).Version(version).Execute()

List Workload versions



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
	workloadId := int64(789) // int64 | The global_id of the Workload resource.
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	version := "version_example" // string | Narrow the list to one version. `latest`, in any case, answers the published version, or an empty list when none is published. Any other value matches a `version_id` and answers an empty list when none matches. An empty value is no filter. A resource that saves and builds in the same request (save and build) publishes no latest version, and `latest` on it answers 400 with code `10000`. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkloadVersionsAPI.ListWorkloadVersions(context.Background(), workloadId).Page(page).PageSize(pageSize).Version(version).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkloadVersionsAPI.ListWorkloadVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListWorkloadVersions`: PaginatedWorkloadVersionList
	fmt.Fprintf(os.Stdout, "Response from `WorkloadVersionsAPI.ListWorkloadVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workloadId** | **int64** | The global_id of the Workload resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListWorkloadVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **version** | **string** | Narrow the list to one version. &#x60;latest&#x60;, in any case, answers the published version, or an empty list when none is published. Any other value matches a &#x60;version_id&#x60; and answers an empty list when none matches. An empty value is no filter. A resource that saves and builds in the same request (save and build) publishes no latest version, and &#x60;latest&#x60; on it answers 400 with code &#x60;10000&#x60;. | 

### Return type

[**PaginatedWorkloadVersionList**](PaginatedWorkloadVersionList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveWorkloadVersion

> WorkloadVersion RetrieveWorkloadVersion(ctx, versionId, workloadId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()

Retrieve a Workload version



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
	versionId := "versionId_example" // string | The short ID identifier of the version.
	workloadId := int64(789) // int64 | The global_id of the Workload resource.
	dependencies := true // bool | Include the resources this version references. (optional)
	dependencyStates := []string{"Inner_example"} // []string | Keep only the dependency versions in these states (comma-separated). Needs dependencies=true. Accepted states: `draft`, `queued`, `building`, `ready`, `error`, `canceled`, `archiving`, `archived`. An unknown state matches nothing, `deleting` and `deleted` match nothing because a dependency version in those states is never listed, and the match is case sensitive (`READY` matches nothing). (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkloadVersionsAPI.RetrieveWorkloadVersion(context.Background(), versionId, workloadId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkloadVersionsAPI.RetrieveWorkloadVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveWorkloadVersion`: WorkloadVersion
	fmt.Fprintf(os.Stdout, "Response from `WorkloadVersionsAPI.RetrieveWorkloadVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**versionId** | **string** | The short ID identifier of the version. | 
**workloadId** | **int64** | The global_id of the Workload resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveWorkloadVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **dependencies** | **bool** | Include the resources this version references. | 
 **dependencyStates** | **[]string** | Keep only the dependency versions in these states (comma-separated). Needs dependencies&#x3D;true. Accepted states: &#x60;draft&#x60;, &#x60;queued&#x60;, &#x60;building&#x60;, &#x60;ready&#x60;, &#x60;error&#x60;, &#x60;canceled&#x60;, &#x60;archiving&#x60;, &#x60;archived&#x60;. An unknown state matches nothing, &#x60;deleting&#x60; and &#x60;deleted&#x60; match nothing because a dependency version in those states is never listed, and the match is case sensitive (&#x60;READY&#x60; matches nothing). | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**WorkloadVersion**](WorkloadVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RevertWorkloadVersion

> WorkloadVersionMeta RevertWorkloadVersion(ctx, versionId, workloadId).WorkloadVersionRevertRequest(workloadVersionRevertRequest).Execute()

Revert to a Workload version



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
	versionId := "versionId_example" // string | The short ID identifier of the version.
	workloadId := int64(789) // int64 | The global_id of the Workload resource.
	workloadVersionRevertRequest := *openapiclient.NewWorkloadVersionRevertRequest() // WorkloadVersionRevertRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkloadVersionsAPI.RevertWorkloadVersion(context.Background(), versionId, workloadId).WorkloadVersionRevertRequest(workloadVersionRevertRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkloadVersionsAPI.RevertWorkloadVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RevertWorkloadVersion`: WorkloadVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `WorkloadVersionsAPI.RevertWorkloadVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**versionId** | **string** | The short ID identifier of the version. | 
**workloadId** | **int64** | The global_id of the Workload resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRevertWorkloadVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **workloadVersionRevertRequest** | [**WorkloadVersionRevertRequest**](WorkloadVersionRevertRequest.md) |  | 

### Return type

[**WorkloadVersionMeta**](WorkloadVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

