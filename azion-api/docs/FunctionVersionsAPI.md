# \FunctionVersionsAPI

All URIs are relative to *https://stage-api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ArchiveFunctionVersion**](FunctionVersionsAPI.md#ArchiveFunctionVersion) | **Post** /workspace/functions/{function_id}/versions/{version_id}/archive | Archive a Function version
[**BuildFunctionVersion**](FunctionVersionsAPI.md#BuildFunctionVersion) | **Post** /workspace/functions/{function_id}/versions/{version_id}/build | Build a Function version
[**CancelFunctionVersionBuild**](FunctionVersionsAPI.md#CancelFunctionVersionBuild) | **Post** /workspace/functions/{function_id}/versions/{version_id}/cancel | Cancel a Function version build
[**CreateFunctionVersion**](FunctionVersionsAPI.md#CreateFunctionVersion) | **Post** /workspace/functions/{function_id}/versions | Create a new Function version
[**DeleteFunctionVersion**](FunctionVersionsAPI.md#DeleteFunctionVersion) | **Delete** /workspace/functions/{function_id}/versions/{version_id} | Delete a Function version
[**ListFunctionVersions**](FunctionVersionsAPI.md#ListFunctionVersions) | **Get** /workspace/functions/{function_id}/versions | List Function versions
[**PartialUpdateFunctionVersion**](FunctionVersionsAPI.md#PartialUpdateFunctionVersion) | **Patch** /workspace/functions/{function_id}/versions/{version_id} | Partially update a Function version
[**RetrieveFunctionVersion**](FunctionVersionsAPI.md#RetrieveFunctionVersion) | **Get** /workspace/functions/{function_id}/versions/{version_id} | Retrieve a Function version
[**UpdateFunctionVersion**](FunctionVersionsAPI.md#UpdateFunctionVersion) | **Put** /workspace/functions/{function_id}/versions/{version_id} | Update a Function version



## ArchiveFunctionVersion

> FunctionVersionMeta ArchiveFunctionVersion(ctx, functionId, versionId).FunctionVersionArchiveRequest(functionVersionArchiveRequest).Execute()

Archive a Function version



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
	functionId := int64(789) // int64 | The ID of the Function resource.
	versionId := "versionId_example" // string | The identifier of the version.
	functionVersionArchiveRequest := *openapiclient.NewFunctionVersionArchiveRequest() // FunctionVersionArchiveRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionVersionsAPI.ArchiveFunctionVersion(context.Background(), functionId, versionId).FunctionVersionArchiveRequest(functionVersionArchiveRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionVersionsAPI.ArchiveFunctionVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ArchiveFunctionVersion`: FunctionVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `FunctionVersionsAPI.ArchiveFunctionVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**functionId** | **int64** | The ID of the Function resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiArchiveFunctionVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **functionVersionArchiveRequest** | [**FunctionVersionArchiveRequest**](FunctionVersionArchiveRequest.md) |  | 

### Return type

[**FunctionVersionMeta**](FunctionVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BuildFunctionVersion

> FunctionVersionMeta BuildFunctionVersion(ctx, functionId, versionId).FunctionVersionBuildRequest(functionVersionBuildRequest).Execute()

Build a Function version



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
	functionId := int64(789) // int64 | The ID of the Function resource.
	versionId := "versionId_example" // string | The identifier of the version.
	functionVersionBuildRequest := *openapiclient.NewFunctionVersionBuildRequest() // FunctionVersionBuildRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionVersionsAPI.BuildFunctionVersion(context.Background(), functionId, versionId).FunctionVersionBuildRequest(functionVersionBuildRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionVersionsAPI.BuildFunctionVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BuildFunctionVersion`: FunctionVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `FunctionVersionsAPI.BuildFunctionVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**functionId** | **int64** | The ID of the Function resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBuildFunctionVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **functionVersionBuildRequest** | [**FunctionVersionBuildRequest**](FunctionVersionBuildRequest.md) |  | 

### Return type

[**FunctionVersionMeta**](FunctionVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelFunctionVersionBuild

> FunctionVersionMeta CancelFunctionVersionBuild(ctx, functionId, versionId).FunctionVersionCancelRequest(functionVersionCancelRequest).Execute()

Cancel a Function version build



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
	functionId := int64(789) // int64 | The ID of the Function resource.
	versionId := "versionId_example" // string | The identifier of the version.
	functionVersionCancelRequest := *openapiclient.NewFunctionVersionCancelRequest() // FunctionVersionCancelRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionVersionsAPI.CancelFunctionVersionBuild(context.Background(), functionId, versionId).FunctionVersionCancelRequest(functionVersionCancelRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionVersionsAPI.CancelFunctionVersionBuild``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelFunctionVersionBuild`: FunctionVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `FunctionVersionsAPI.CancelFunctionVersionBuild`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**functionId** | **int64** | The ID of the Function resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelFunctionVersionBuildRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **functionVersionCancelRequest** | [**FunctionVersionCancelRequest**](FunctionVersionCancelRequest.md) |  | 

### Return type

[**FunctionVersionMeta**](FunctionVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateFunctionVersion

> FunctionVersion CreateFunctionVersion(ctx, functionId).FunctionVersionCreateRequest(functionVersionCreateRequest).Execute()

Create a new Function version



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
	functionId := int64(789) // int64 | The ID of the Function resource.
	functionVersionCreateRequest := *openapiclient.NewFunctionVersionCreateRequest() // FunctionVersionCreateRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionVersionsAPI.CreateFunctionVersion(context.Background(), functionId).FunctionVersionCreateRequest(functionVersionCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionVersionsAPI.CreateFunctionVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateFunctionVersion`: FunctionVersion
	fmt.Fprintf(os.Stdout, "Response from `FunctionVersionsAPI.CreateFunctionVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**functionId** | **int64** | The ID of the Function resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateFunctionVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **functionVersionCreateRequest** | [**FunctionVersionCreateRequest**](FunctionVersionCreateRequest.md) |  | 

### Return type

[**FunctionVersion**](FunctionVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteFunctionVersion

> FunctionVersionMeta DeleteFunctionVersion(ctx, functionId, versionId).Execute()

Delete a Function version



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
	functionId := int64(789) // int64 | The ID of the Function resource.
	versionId := "versionId_example" // string | The identifier of the version.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionVersionsAPI.DeleteFunctionVersion(context.Background(), functionId, versionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionVersionsAPI.DeleteFunctionVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteFunctionVersion`: FunctionVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `FunctionVersionsAPI.DeleteFunctionVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**functionId** | **int64** | The ID of the Function resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteFunctionVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**FunctionVersionMeta**](FunctionVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListFunctionVersions

> PaginatedFunctionVersionList ListFunctionVersions(ctx, functionId).Page(page).PageSize(pageSize).Execute()

List Function versions



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
	functionId := int64(789) // int64 | The ID of the Function resource.
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionVersionsAPI.ListFunctionVersions(context.Background(), functionId).Page(page).PageSize(pageSize).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionVersionsAPI.ListFunctionVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListFunctionVersions`: PaginatedFunctionVersionList
	fmt.Fprintf(os.Stdout, "Response from `FunctionVersionsAPI.ListFunctionVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**functionId** | **int64** | The ID of the Function resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListFunctionVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 

### Return type

[**PaginatedFunctionVersionList**](PaginatedFunctionVersionList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateFunctionVersion

> FunctionVersion PartialUpdateFunctionVersion(ctx, functionId, versionId).PatchedFunctionRequest(patchedFunctionRequest).Execute()

Partially update a Function version



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
	functionId := int64(789) // int64 | The ID of the Function resource.
	versionId := "versionId_example" // string | The identifier of the version.
	patchedFunctionRequest := *openapiclient.NewPatchedFunctionRequest() // PatchedFunctionRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionVersionsAPI.PartialUpdateFunctionVersion(context.Background(), functionId, versionId).PatchedFunctionRequest(patchedFunctionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionVersionsAPI.PartialUpdateFunctionVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateFunctionVersion`: FunctionVersion
	fmt.Fprintf(os.Stdout, "Response from `FunctionVersionsAPI.PartialUpdateFunctionVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**functionId** | **int64** | The ID of the Function resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateFunctionVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **patchedFunctionRequest** | [**PatchedFunctionRequest**](PatchedFunctionRequest.md) |  | 

### Return type

[**FunctionVersion**](FunctionVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveFunctionVersion

> FunctionVersion RetrieveFunctionVersion(ctx, functionId, versionId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()

Retrieve a Function version



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
	functionId := int64(789) // int64 | The ID of the Function resource.
	versionId := "versionId_example" // string | The identifier of the version.
	dependencies := true // bool | Include the resources this version references. (optional)
	dependencyStates := []string{"Inner_example"} // []string | Keep only the dependency versions in these states (comma-separated). Needs dependencies=true. Accepted states: `draft`, `queued`, `building`, `ready`, `error`, `canceled`, `archiving`, `archived`. An unknown state matches nothing, `deleting` and `deleted` match nothing because a dependency version in those states is never listed, and the match is case sensitive (`READY` matches nothing). (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionVersionsAPI.RetrieveFunctionVersion(context.Background(), functionId, versionId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionVersionsAPI.RetrieveFunctionVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveFunctionVersion`: FunctionVersion
	fmt.Fprintf(os.Stdout, "Response from `FunctionVersionsAPI.RetrieveFunctionVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**functionId** | **int64** | The ID of the Function resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveFunctionVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **dependencies** | **bool** | Include the resources this version references. | 
 **dependencyStates** | **[]string** | Keep only the dependency versions in these states (comma-separated). Needs dependencies&#x3D;true. Accepted states: &#x60;draft&#x60;, &#x60;queued&#x60;, &#x60;building&#x60;, &#x60;ready&#x60;, &#x60;error&#x60;, &#x60;canceled&#x60;, &#x60;archiving&#x60;, &#x60;archived&#x60;. An unknown state matches nothing, &#x60;deleting&#x60; and &#x60;deleted&#x60; match nothing because a dependency version in those states is never listed, and the match is case sensitive (&#x60;READY&#x60; matches nothing). | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**FunctionVersion**](FunctionVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateFunctionVersion

> FunctionVersion UpdateFunctionVersion(ctx, functionId, versionId).FunctionRequest(functionRequest).Execute()

Update a Function version



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
	functionId := int64(789) // int64 | The ID of the Function resource.
	versionId := "versionId_example" // string | The identifier of the version.
	functionRequest := *openapiclient.NewFunctionRequest("Name_example", "Code_example") // FunctionRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FunctionVersionsAPI.UpdateFunctionVersion(context.Background(), functionId, versionId).FunctionRequest(functionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FunctionVersionsAPI.UpdateFunctionVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateFunctionVersion`: FunctionVersion
	fmt.Fprintf(os.Stdout, "Response from `FunctionVersionsAPI.UpdateFunctionVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**functionId** | **int64** | The ID of the Function resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateFunctionVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **functionRequest** | [**FunctionRequest**](FunctionRequest.md) |  | 

### Return type

[**FunctionVersion**](FunctionVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

