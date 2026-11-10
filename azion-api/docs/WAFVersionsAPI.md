# \WAFVersionsAPI

All URIs are relative to *https://stage-api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ArchiveWafVersion**](WAFVersionsAPI.md#ArchiveWafVersion) | **Post** /workspace/wafs/{waf_id}/versions/{version_id}/archive | Archive a WAF version
[**BuildWafVersion**](WAFVersionsAPI.md#BuildWafVersion) | **Post** /workspace/wafs/{waf_id}/versions/{version_id}/build | Build a WAF version
[**CancelWafVersionBuild**](WAFVersionsAPI.md#CancelWafVersionBuild) | **Post** /workspace/wafs/{waf_id}/versions/{version_id}/cancel | Cancel a WAF version build
[**CreateWafVersion**](WAFVersionsAPI.md#CreateWafVersion) | **Post** /workspace/wafs/{waf_id}/versions | Create a new WAF version
[**DeleteWafVersion**](WAFVersionsAPI.md#DeleteWafVersion) | **Delete** /workspace/wafs/{waf_id}/versions/{version_id} | Delete a WAF version
[**ListWafVersions**](WAFVersionsAPI.md#ListWafVersions) | **Get** /workspace/wafs/{waf_id}/versions | List WAF versions
[**PartialUpdateWafVersion**](WAFVersionsAPI.md#PartialUpdateWafVersion) | **Patch** /workspace/wafs/{waf_id}/versions/{version_id} | Partially update a WAF version
[**RetrieveWafVersion**](WAFVersionsAPI.md#RetrieveWafVersion) | **Get** /workspace/wafs/{waf_id}/versions/{version_id} | Retrieve a WAF version
[**UpdateWafVersion**](WAFVersionsAPI.md#UpdateWafVersion) | **Put** /workspace/wafs/{waf_id}/versions/{version_id} | Update a WAF version



## ArchiveWafVersion

> WAFVersionMeta ArchiveWafVersion(ctx, versionId, wafId).WAFVersionArchiveRequest(wAFVersionArchiveRequest).Execute()

Archive a WAF version



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
	versionId := "versionId_example" // string | The identifier of the version.
	wafId := int64(789) // int64 | The ID of the WAF resource.
	wAFVersionArchiveRequest := *openapiclient.NewWAFVersionArchiveRequest() // WAFVersionArchiveRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WAFVersionsAPI.ArchiveWafVersion(context.Background(), versionId, wafId).WAFVersionArchiveRequest(wAFVersionArchiveRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WAFVersionsAPI.ArchiveWafVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ArchiveWafVersion`: WAFVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `WAFVersionsAPI.ArchiveWafVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**versionId** | **string** | The identifier of the version. | 
**wafId** | **int64** | The ID of the WAF resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiArchiveWafVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **wAFVersionArchiveRequest** | [**WAFVersionArchiveRequest**](WAFVersionArchiveRequest.md) |  | 

### Return type

[**WAFVersionMeta**](WAFVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BuildWafVersion

> WAFVersionMeta BuildWafVersion(ctx, versionId, wafId).WAFVersionBuildRequest(wAFVersionBuildRequest).Execute()

Build a WAF version



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
	versionId := "versionId_example" // string | The identifier of the version.
	wafId := int64(789) // int64 | The ID of the WAF resource.
	wAFVersionBuildRequest := *openapiclient.NewWAFVersionBuildRequest() // WAFVersionBuildRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WAFVersionsAPI.BuildWafVersion(context.Background(), versionId, wafId).WAFVersionBuildRequest(wAFVersionBuildRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WAFVersionsAPI.BuildWafVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BuildWafVersion`: WAFVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `WAFVersionsAPI.BuildWafVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**versionId** | **string** | The identifier of the version. | 
**wafId** | **int64** | The ID of the WAF resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBuildWafVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **wAFVersionBuildRequest** | [**WAFVersionBuildRequest**](WAFVersionBuildRequest.md) |  | 

### Return type

[**WAFVersionMeta**](WAFVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelWafVersionBuild

> WAFVersionMeta CancelWafVersionBuild(ctx, versionId, wafId).WAFVersionCancelRequest(wAFVersionCancelRequest).Execute()

Cancel a WAF version build



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
	versionId := "versionId_example" // string | The identifier of the version.
	wafId := int64(789) // int64 | The ID of the WAF resource.
	wAFVersionCancelRequest := *openapiclient.NewWAFVersionCancelRequest() // WAFVersionCancelRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WAFVersionsAPI.CancelWafVersionBuild(context.Background(), versionId, wafId).WAFVersionCancelRequest(wAFVersionCancelRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WAFVersionsAPI.CancelWafVersionBuild``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelWafVersionBuild`: WAFVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `WAFVersionsAPI.CancelWafVersionBuild`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**versionId** | **string** | The identifier of the version. | 
**wafId** | **int64** | The ID of the WAF resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelWafVersionBuildRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **wAFVersionCancelRequest** | [**WAFVersionCancelRequest**](WAFVersionCancelRequest.md) |  | 

### Return type

[**WAFVersionMeta**](WAFVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateWafVersion

> WAFVersion CreateWafVersion(ctx, wafId).WAFVersionCreateRequest(wAFVersionCreateRequest).Execute()

Create a new WAF version



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
	wafId := int64(789) // int64 | The ID of the WAF resource.
	wAFVersionCreateRequest := *openapiclient.NewWAFVersionCreateRequest() // WAFVersionCreateRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WAFVersionsAPI.CreateWafVersion(context.Background(), wafId).WAFVersionCreateRequest(wAFVersionCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WAFVersionsAPI.CreateWafVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateWafVersion`: WAFVersion
	fmt.Fprintf(os.Stdout, "Response from `WAFVersionsAPI.CreateWafVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**wafId** | **int64** | The ID of the WAF resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateWafVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **wAFVersionCreateRequest** | [**WAFVersionCreateRequest**](WAFVersionCreateRequest.md) |  | 

### Return type

[**WAFVersion**](WAFVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteWafVersion

> WAFVersionMeta DeleteWafVersion(ctx, versionId, wafId).Execute()

Delete a WAF version



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
	versionId := "versionId_example" // string | The identifier of the version.
	wafId := int64(789) // int64 | The ID of the WAF resource.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WAFVersionsAPI.DeleteWafVersion(context.Background(), versionId, wafId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WAFVersionsAPI.DeleteWafVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteWafVersion`: WAFVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `WAFVersionsAPI.DeleteWafVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**versionId** | **string** | The identifier of the version. | 
**wafId** | **int64** | The ID of the WAF resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteWafVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**WAFVersionMeta**](WAFVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListWafVersions

> PaginatedWAFVersionList ListWafVersions(ctx, wafId).Page(page).PageSize(pageSize).Execute()

List WAF versions



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
	wafId := int64(789) // int64 | The ID of the WAF resource.
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WAFVersionsAPI.ListWafVersions(context.Background(), wafId).Page(page).PageSize(pageSize).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WAFVersionsAPI.ListWafVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListWafVersions`: PaginatedWAFVersionList
	fmt.Fprintf(os.Stdout, "Response from `WAFVersionsAPI.ListWafVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**wafId** | **int64** | The ID of the WAF resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListWafVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 

### Return type

[**PaginatedWAFVersionList**](PaginatedWAFVersionList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateWafVersion

> WAFVersion PartialUpdateWafVersion(ctx, versionId, wafId).PatchedWAFRequest(patchedWAFRequest).Execute()

Partially update a WAF version



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
	versionId := "versionId_example" // string | The identifier of the version.
	wafId := int64(789) // int64 | The ID of the WAF resource.
	patchedWAFRequest := *openapiclient.NewPatchedWAFRequest() // PatchedWAFRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WAFVersionsAPI.PartialUpdateWafVersion(context.Background(), versionId, wafId).PatchedWAFRequest(patchedWAFRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WAFVersionsAPI.PartialUpdateWafVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateWafVersion`: WAFVersion
	fmt.Fprintf(os.Stdout, "Response from `WAFVersionsAPI.PartialUpdateWafVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**versionId** | **string** | The identifier of the version. | 
**wafId** | **int64** | The ID of the WAF resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateWafVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **patchedWAFRequest** | [**PatchedWAFRequest**](PatchedWAFRequest.md) |  | 

### Return type

[**WAFVersion**](WAFVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveWafVersion

> WAFVersion RetrieveWafVersion(ctx, versionId, wafId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()

Retrieve a WAF version



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
	versionId := "versionId_example" // string | The identifier of the version.
	wafId := int64(789) // int64 | The ID of the WAF resource.
	dependencies := true // bool | Include the resources this version references. (optional)
	dependencyStates := []string{"Inner_example"} // []string | Keep only the dependency versions in these states (comma-separated). Needs dependencies=true. (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WAFVersionsAPI.RetrieveWafVersion(context.Background(), versionId, wafId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WAFVersionsAPI.RetrieveWafVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveWafVersion`: WAFVersion
	fmt.Fprintf(os.Stdout, "Response from `WAFVersionsAPI.RetrieveWafVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**versionId** | **string** | The identifier of the version. | 
**wafId** | **int64** | The ID of the WAF resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveWafVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **dependencies** | **bool** | Include the resources this version references. | 
 **dependencyStates** | **[]string** | Keep only the dependency versions in these states (comma-separated). Needs dependencies&#x3D;true. | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**WAFVersion**](WAFVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateWafVersion

> WAFVersion UpdateWafVersion(ctx, versionId, wafId).WAFRequest(wAFRequest).Execute()

Update a WAF version



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
	versionId := "versionId_example" // string | The identifier of the version.
	wafId := int64(789) // int64 | The ID of the WAF resource.
	wAFRequest := *openapiclient.NewWAFRequest("Name_example") // WAFRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WAFVersionsAPI.UpdateWafVersion(context.Background(), versionId, wafId).WAFRequest(wAFRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WAFVersionsAPI.UpdateWafVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateWafVersion`: WAFVersion
	fmt.Fprintf(os.Stdout, "Response from `WAFVersionsAPI.UpdateWafVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**versionId** | **string** | The identifier of the version. | 
**wafId** | **int64** | The ID of the WAF resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateWafVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **wAFRequest** | [**WAFRequest**](WAFRequest.md) |  | 

### Return type

[**WAFVersion**](WAFVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

