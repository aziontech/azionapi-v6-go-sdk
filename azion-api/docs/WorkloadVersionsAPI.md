# \WorkloadVersionsAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListWorkloadVersions**](WorkloadVersionsAPI.md#ListWorkloadVersions) | **Get** /workspace/workloads/{resource_pk}/versions | List Workload versions
[**RetrieveWorkloadVersion**](WorkloadVersionsAPI.md#RetrieveWorkloadVersion) | **Get** /workspace/workloads/{resource_pk}/versions/{id} | Retrieve a Workload version
[**RevertWorkloadVersion**](WorkloadVersionsAPI.md#RevertWorkloadVersion) | **Post** /workspace/workloads/{resource_pk}/versions/{id}/revert | Revert to a Workload version



## ListWorkloadVersions

> PaginatedWorkloadList ListWorkloadVersions(ctx, resourcePk).Fields(fields).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()

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
	resourcePk := int64(789) // int64 | The global_id of the Workload resource.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	ordering := "ordering_example" // string | Which field to use when ordering the results. (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	search := "search_example" // string | A search term. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkloadVersionsAPI.ListWorkloadVersions(context.Background(), resourcePk).Fields(fields).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkloadVersionsAPI.ListWorkloadVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListWorkloadVersions`: PaginatedWorkloadList
	fmt.Fprintf(os.Stdout, "Response from `WorkloadVersionsAPI.ListWorkloadVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**resourcePk** | **int64** | The global_id of the Workload resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListWorkloadVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **ordering** | **string** | Which field to use when ordering the results. | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **search** | **string** | A search term. | 

### Return type

[**PaginatedWorkloadList**](PaginatedWorkloadList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveWorkloadVersion

> Workload RetrieveWorkloadVersion(ctx, id, resourcePk).Fields(fields).Execute()

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
	id := "id_example" // string | The short ID identifier of the version.
	resourcePk := int64(789) // int64 | The global_id of the Workload resource.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkloadVersionsAPI.RetrieveWorkloadVersion(context.Background(), id, resourcePk).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkloadVersionsAPI.RetrieveWorkloadVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveWorkloadVersion`: Workload
	fmt.Fprintf(os.Stdout, "Response from `WorkloadVersionsAPI.RetrieveWorkloadVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | The short ID identifier of the version. | 
**resourcePk** | **int64** | The global_id of the Workload resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveWorkloadVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**Workload**](Workload.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RevertWorkloadVersion

> RevertWorkloadVersion(ctx, id, resourcePk).VersionRevertRequest(versionRevertRequest).Execute()

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
	id := "id_example" // string | The short ID identifier of the version.
	resourcePk := int64(789) // int64 | The global_id of the Workload resource.
	versionRevertRequest := *openapiclient.NewVersionRevertRequest() // VersionRevertRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.WorkloadVersionsAPI.RevertWorkloadVersion(context.Background(), id, resourcePk).VersionRevertRequest(versionRevertRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkloadVersionsAPI.RevertWorkloadVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | The short ID identifier of the version. | 
**resourcePk** | **int64** | The global_id of the Workload resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRevertWorkloadVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **versionRevertRequest** | [**VersionRevertRequest**](VersionRevertRequest.md) |  | 

### Return type

 (empty response body)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

