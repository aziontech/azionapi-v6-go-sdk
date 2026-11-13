# \CustomPageVersionsAPI

All URIs are relative to *https://stage-api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ArchiveCustomPageVersion**](CustomPageVersionsAPI.md#ArchiveCustomPageVersion) | **Post** /workspace/custom_pages/{custom_page_id}/versions/{version_id}/archive | Archive a Custom Page version
[**BuildCustomPageVersion**](CustomPageVersionsAPI.md#BuildCustomPageVersion) | **Post** /workspace/custom_pages/{custom_page_id}/versions/{version_id}/build | Build a Custom Page version
[**CancelCustomPageVersionBuild**](CustomPageVersionsAPI.md#CancelCustomPageVersionBuild) | **Post** /workspace/custom_pages/{custom_page_id}/versions/{version_id}/cancel | Cancel a Custom Page version build
[**CreateCustomPageVersion**](CustomPageVersionsAPI.md#CreateCustomPageVersion) | **Post** /workspace/custom_pages/{custom_page_id}/versions | Create a new Custom Page version
[**DeleteCustomPageVersion**](CustomPageVersionsAPI.md#DeleteCustomPageVersion) | **Delete** /workspace/custom_pages/{custom_page_id}/versions/{version_id} | Delete a Custom Page version
[**ListCustomPageVersions**](CustomPageVersionsAPI.md#ListCustomPageVersions) | **Get** /workspace/custom_pages/{custom_page_id}/versions | List Custom Page versions
[**PartialUpdateCustomPageVersion**](CustomPageVersionsAPI.md#PartialUpdateCustomPageVersion) | **Patch** /workspace/custom_pages/{custom_page_id}/versions/{version_id} | Partially update a Custom Page version
[**RetrieveCustomPageVersion**](CustomPageVersionsAPI.md#RetrieveCustomPageVersion) | **Get** /workspace/custom_pages/{custom_page_id}/versions/{version_id} | Retrieve a Custom Page version
[**UpdateCustomPageVersion**](CustomPageVersionsAPI.md#UpdateCustomPageVersion) | **Put** /workspace/custom_pages/{custom_page_id}/versions/{version_id} | Update a Custom Page version



## ArchiveCustomPageVersion

> CustomPageVersionMeta ArchiveCustomPageVersion(ctx, customPageId, versionId).CustomPageVersionArchiveRequest(customPageVersionArchiveRequest).Execute()

Archive a Custom Page version



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
	customPageId := int64(789) // int64 | The ID of the Custom Page resource.
	versionId := "versionId_example" // string | The identifier of the version.
	customPageVersionArchiveRequest := *openapiclient.NewCustomPageVersionArchiveRequest() // CustomPageVersionArchiveRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomPageVersionsAPI.ArchiveCustomPageVersion(context.Background(), customPageId, versionId).CustomPageVersionArchiveRequest(customPageVersionArchiveRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomPageVersionsAPI.ArchiveCustomPageVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ArchiveCustomPageVersion`: CustomPageVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `CustomPageVersionsAPI.ArchiveCustomPageVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**customPageId** | **int64** | The ID of the Custom Page resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiArchiveCustomPageVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **customPageVersionArchiveRequest** | [**CustomPageVersionArchiveRequest**](CustomPageVersionArchiveRequest.md) |  | 

### Return type

[**CustomPageVersionMeta**](CustomPageVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BuildCustomPageVersion

> CustomPageVersionMeta BuildCustomPageVersion(ctx, customPageId, versionId).CustomPageVersionBuildRequest(customPageVersionBuildRequest).Execute()

Build a Custom Page version



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
	customPageId := int64(789) // int64 | The ID of the Custom Page resource.
	versionId := "versionId_example" // string | The identifier of the version.
	customPageVersionBuildRequest := *openapiclient.NewCustomPageVersionBuildRequest() // CustomPageVersionBuildRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomPageVersionsAPI.BuildCustomPageVersion(context.Background(), customPageId, versionId).CustomPageVersionBuildRequest(customPageVersionBuildRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomPageVersionsAPI.BuildCustomPageVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BuildCustomPageVersion`: CustomPageVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `CustomPageVersionsAPI.BuildCustomPageVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**customPageId** | **int64** | The ID of the Custom Page resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBuildCustomPageVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **customPageVersionBuildRequest** | [**CustomPageVersionBuildRequest**](CustomPageVersionBuildRequest.md) |  | 

### Return type

[**CustomPageVersionMeta**](CustomPageVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelCustomPageVersionBuild

> CustomPageVersionMeta CancelCustomPageVersionBuild(ctx, customPageId, versionId).CustomPageVersionCancelRequest(customPageVersionCancelRequest).Execute()

Cancel a Custom Page version build



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
	customPageId := int64(789) // int64 | The ID of the Custom Page resource.
	versionId := "versionId_example" // string | The identifier of the version.
	customPageVersionCancelRequest := *openapiclient.NewCustomPageVersionCancelRequest() // CustomPageVersionCancelRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomPageVersionsAPI.CancelCustomPageVersionBuild(context.Background(), customPageId, versionId).CustomPageVersionCancelRequest(customPageVersionCancelRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomPageVersionsAPI.CancelCustomPageVersionBuild``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelCustomPageVersionBuild`: CustomPageVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `CustomPageVersionsAPI.CancelCustomPageVersionBuild`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**customPageId** | **int64** | The ID of the Custom Page resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelCustomPageVersionBuildRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **customPageVersionCancelRequest** | [**CustomPageVersionCancelRequest**](CustomPageVersionCancelRequest.md) |  | 

### Return type

[**CustomPageVersionMeta**](CustomPageVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateCustomPageVersion

> CustomPageVersion CreateCustomPageVersion(ctx, customPageId).CustomPageVersionCreateRequest(customPageVersionCreateRequest).Execute()

Create a new Custom Page version



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
	customPageId := int64(789) // int64 | The ID of the Custom Page resource.
	customPageVersionCreateRequest := *openapiclient.NewCustomPageVersionCreateRequest() // CustomPageVersionCreateRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomPageVersionsAPI.CreateCustomPageVersion(context.Background(), customPageId).CustomPageVersionCreateRequest(customPageVersionCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomPageVersionsAPI.CreateCustomPageVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateCustomPageVersion`: CustomPageVersion
	fmt.Fprintf(os.Stdout, "Response from `CustomPageVersionsAPI.CreateCustomPageVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**customPageId** | **int64** | The ID of the Custom Page resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateCustomPageVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **customPageVersionCreateRequest** | [**CustomPageVersionCreateRequest**](CustomPageVersionCreateRequest.md) |  | 

### Return type

[**CustomPageVersion**](CustomPageVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteCustomPageVersion

> CustomPageVersionMeta DeleteCustomPageVersion(ctx, customPageId, versionId).Execute()

Delete a Custom Page version



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
	customPageId := int64(789) // int64 | The ID of the Custom Page resource.
	versionId := "versionId_example" // string | The identifier of the version.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomPageVersionsAPI.DeleteCustomPageVersion(context.Background(), customPageId, versionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomPageVersionsAPI.DeleteCustomPageVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteCustomPageVersion`: CustomPageVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `CustomPageVersionsAPI.DeleteCustomPageVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**customPageId** | **int64** | The ID of the Custom Page resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteCustomPageVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**CustomPageVersionMeta**](CustomPageVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCustomPageVersions

> PaginatedCustomPageVersionList ListCustomPageVersions(ctx, customPageId).Page(page).PageSize(pageSize).Version(version).Execute()

List Custom Page versions



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
	customPageId := int64(789) // int64 | The ID of the Custom Page resource.
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	version := "version_example" // string | Narrow the list to one version. `latest`, in any case, answers the published version, or an empty list when none is published. Any other value matches a `version_id` and answers an empty list when none matches. An empty value is no filter. A resource that saves and builds in the same request (save and build) publishes no latest version, and `latest` on it answers 400 with code `10000`. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomPageVersionsAPI.ListCustomPageVersions(context.Background(), customPageId).Page(page).PageSize(pageSize).Version(version).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomPageVersionsAPI.ListCustomPageVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCustomPageVersions`: PaginatedCustomPageVersionList
	fmt.Fprintf(os.Stdout, "Response from `CustomPageVersionsAPI.ListCustomPageVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**customPageId** | **int64** | The ID of the Custom Page resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListCustomPageVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **version** | **string** | Narrow the list to one version. &#x60;latest&#x60;, in any case, answers the published version, or an empty list when none is published. Any other value matches a &#x60;version_id&#x60; and answers an empty list when none matches. An empty value is no filter. A resource that saves and builds in the same request (save and build) publishes no latest version, and &#x60;latest&#x60; on it answers 400 with code &#x60;10000&#x60;. | 

### Return type

[**PaginatedCustomPageVersionList**](PaginatedCustomPageVersionList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateCustomPageVersion

> CustomPageVersion PartialUpdateCustomPageVersion(ctx, customPageId, versionId).PatchedCustomPageRequest(patchedCustomPageRequest).Execute()

Partially update a Custom Page version



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
	customPageId := int64(789) // int64 | The ID of the Custom Page resource.
	versionId := "versionId_example" // string | The identifier of the version.
	patchedCustomPageRequest := *openapiclient.NewPatchedCustomPageRequest() // PatchedCustomPageRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomPageVersionsAPI.PartialUpdateCustomPageVersion(context.Background(), customPageId, versionId).PatchedCustomPageRequest(patchedCustomPageRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomPageVersionsAPI.PartialUpdateCustomPageVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateCustomPageVersion`: CustomPageVersion
	fmt.Fprintf(os.Stdout, "Response from `CustomPageVersionsAPI.PartialUpdateCustomPageVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**customPageId** | **int64** | The ID of the Custom Page resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateCustomPageVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **patchedCustomPageRequest** | [**PatchedCustomPageRequest**](PatchedCustomPageRequest.md) |  | 

### Return type

[**CustomPageVersion**](CustomPageVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveCustomPageVersion

> CustomPageVersion RetrieveCustomPageVersion(ctx, customPageId, versionId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()

Retrieve a Custom Page version



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
	customPageId := int64(789) // int64 | The ID of the Custom Page resource.
	versionId := "versionId_example" // string | The identifier of the version.
	dependencies := true // bool | Include the resources this version references. (optional)
	dependencyStates := []string{"Inner_example"} // []string | Keep only the dependency versions in these states (comma-separated). Needs dependencies=true. Accepted states: `draft`, `queued`, `building`, `ready`, `error`, `canceled`, `archiving`, `archived`. An unknown state matches nothing, `deleting` and `deleted` match nothing because a dependency version in those states is never listed, and the match is case sensitive (`READY` matches nothing). (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomPageVersionsAPI.RetrieveCustomPageVersion(context.Background(), customPageId, versionId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomPageVersionsAPI.RetrieveCustomPageVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveCustomPageVersion`: CustomPageVersion
	fmt.Fprintf(os.Stdout, "Response from `CustomPageVersionsAPI.RetrieveCustomPageVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**customPageId** | **int64** | The ID of the Custom Page resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveCustomPageVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **dependencies** | **bool** | Include the resources this version references. | 
 **dependencyStates** | **[]string** | Keep only the dependency versions in these states (comma-separated). Needs dependencies&#x3D;true. Accepted states: &#x60;draft&#x60;, &#x60;queued&#x60;, &#x60;building&#x60;, &#x60;ready&#x60;, &#x60;error&#x60;, &#x60;canceled&#x60;, &#x60;archiving&#x60;, &#x60;archived&#x60;. An unknown state matches nothing, &#x60;deleting&#x60; and &#x60;deleted&#x60; match nothing because a dependency version in those states is never listed, and the match is case sensitive (&#x60;READY&#x60; matches nothing). | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**CustomPageVersion**](CustomPageVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateCustomPageVersion

> CustomPageVersion UpdateCustomPageVersion(ctx, customPageId, versionId).CustomPageRequest(customPageRequest).Execute()

Update a Custom Page version



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
	customPageId := int64(789) // int64 | The ID of the Custom Page resource.
	versionId := "versionId_example" // string | The identifier of the version.
	customPageRequest := *openapiclient.NewCustomPageRequest("Name_example", []openapiclient.PageRequest{*openapiclient.NewPageRequest("Code_example", *openapiclient.NewPageConnectorRequest("Type_example", *openapiclient.NewPageConnectorAttributesRequest(int32(123))))}) // CustomPageRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CustomPageVersionsAPI.UpdateCustomPageVersion(context.Background(), customPageId, versionId).CustomPageRequest(customPageRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CustomPageVersionsAPI.UpdateCustomPageVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateCustomPageVersion`: CustomPageVersion
	fmt.Fprintf(os.Stdout, "Response from `CustomPageVersionsAPI.UpdateCustomPageVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**customPageId** | **int64** | The ID of the Custom Page resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateCustomPageVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **customPageRequest** | [**CustomPageRequest**](CustomPageRequest.md) |  | 

### Return type

[**CustomPageVersion**](CustomPageVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

