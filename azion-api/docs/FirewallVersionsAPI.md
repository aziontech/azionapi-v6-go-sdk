# \FirewallVersionsAPI

All URIs are relative to *https://stage-api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ArchiveFirewallVersion**](FirewallVersionsAPI.md#ArchiveFirewallVersion) | **Post** /workspace/firewalls/{firewall_id}/versions/{version_id}/archive | Archive a Firewall version
[**BuildFirewallVersion**](FirewallVersionsAPI.md#BuildFirewallVersion) | **Post** /workspace/firewalls/{firewall_id}/versions/{version_id}/build | Build a Firewall version
[**CancelFirewallVersionBuild**](FirewallVersionsAPI.md#CancelFirewallVersionBuild) | **Post** /workspace/firewalls/{firewall_id}/versions/{version_id}/cancel | Cancel a Firewall version build
[**CreateFirewallVersion**](FirewallVersionsAPI.md#CreateFirewallVersion) | **Post** /workspace/firewalls/{firewall_id}/versions | Create a new Firewall version
[**DeleteFirewallVersion**](FirewallVersionsAPI.md#DeleteFirewallVersion) | **Delete** /workspace/firewalls/{firewall_id}/versions/{version_id} | Delete a Firewall version
[**ListFirewallVersions**](FirewallVersionsAPI.md#ListFirewallVersions) | **Get** /workspace/firewalls/{firewall_id}/versions | List Firewall versions
[**PartialUpdateFirewallVersion**](FirewallVersionsAPI.md#PartialUpdateFirewallVersion) | **Patch** /workspace/firewalls/{firewall_id}/versions/{version_id} | Partially update a Firewall version
[**RetrieveFirewallVersion**](FirewallVersionsAPI.md#RetrieveFirewallVersion) | **Get** /workspace/firewalls/{firewall_id}/versions/{version_id} | Retrieve a Firewall version
[**UpdateFirewallVersion**](FirewallVersionsAPI.md#UpdateFirewallVersion) | **Put** /workspace/firewalls/{firewall_id}/versions/{version_id} | Update a Firewall version



## ArchiveFirewallVersion

> FirewallVersionMeta ArchiveFirewallVersion(ctx, firewallId, versionId).FirewallVersionArchiveRequest(firewallVersionArchiveRequest).Execute()

Archive a Firewall version



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
	firewallId := int64(789) // int64 | The ID of the Firewall resource.
	versionId := "versionId_example" // string | The identifier of the version.
	firewallVersionArchiveRequest := *openapiclient.NewFirewallVersionArchiveRequest() // FirewallVersionArchiveRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallVersionsAPI.ArchiveFirewallVersion(context.Background(), firewallId, versionId).FirewallVersionArchiveRequest(firewallVersionArchiveRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallVersionsAPI.ArchiveFirewallVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ArchiveFirewallVersion`: FirewallVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `FirewallVersionsAPI.ArchiveFirewallVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | The ID of the Firewall resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiArchiveFirewallVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **firewallVersionArchiveRequest** | [**FirewallVersionArchiveRequest**](FirewallVersionArchiveRequest.md) |  | 

### Return type

[**FirewallVersionMeta**](FirewallVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BuildFirewallVersion

> FirewallVersionMeta BuildFirewallVersion(ctx, firewallId, versionId).FirewallVersionBuildRequest(firewallVersionBuildRequest).Execute()

Build a Firewall version



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
	firewallId := int64(789) // int64 | The ID of the Firewall resource.
	versionId := "versionId_example" // string | The identifier of the version.
	firewallVersionBuildRequest := *openapiclient.NewFirewallVersionBuildRequest() // FirewallVersionBuildRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallVersionsAPI.BuildFirewallVersion(context.Background(), firewallId, versionId).FirewallVersionBuildRequest(firewallVersionBuildRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallVersionsAPI.BuildFirewallVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BuildFirewallVersion`: FirewallVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `FirewallVersionsAPI.BuildFirewallVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | The ID of the Firewall resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBuildFirewallVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **firewallVersionBuildRequest** | [**FirewallVersionBuildRequest**](FirewallVersionBuildRequest.md) |  | 

### Return type

[**FirewallVersionMeta**](FirewallVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelFirewallVersionBuild

> FirewallVersionMeta CancelFirewallVersionBuild(ctx, firewallId, versionId).FirewallVersionCancelRequest(firewallVersionCancelRequest).Execute()

Cancel a Firewall version build



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
	firewallId := int64(789) // int64 | The ID of the Firewall resource.
	versionId := "versionId_example" // string | The identifier of the version.
	firewallVersionCancelRequest := *openapiclient.NewFirewallVersionCancelRequest() // FirewallVersionCancelRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallVersionsAPI.CancelFirewallVersionBuild(context.Background(), firewallId, versionId).FirewallVersionCancelRequest(firewallVersionCancelRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallVersionsAPI.CancelFirewallVersionBuild``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelFirewallVersionBuild`: FirewallVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `FirewallVersionsAPI.CancelFirewallVersionBuild`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | The ID of the Firewall resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelFirewallVersionBuildRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **firewallVersionCancelRequest** | [**FirewallVersionCancelRequest**](FirewallVersionCancelRequest.md) |  | 

### Return type

[**FirewallVersionMeta**](FirewallVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateFirewallVersion

> FirewallVersion CreateFirewallVersion(ctx, firewallId).FirewallVersionCreateRequest(firewallVersionCreateRequest).Execute()

Create a new Firewall version



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
	firewallId := int64(789) // int64 | The ID of the Firewall resource.
	firewallVersionCreateRequest := *openapiclient.NewFirewallVersionCreateRequest() // FirewallVersionCreateRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallVersionsAPI.CreateFirewallVersion(context.Background(), firewallId).FirewallVersionCreateRequest(firewallVersionCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallVersionsAPI.CreateFirewallVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateFirewallVersion`: FirewallVersion
	fmt.Fprintf(os.Stdout, "Response from `FirewallVersionsAPI.CreateFirewallVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | The ID of the Firewall resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateFirewallVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **firewallVersionCreateRequest** | [**FirewallVersionCreateRequest**](FirewallVersionCreateRequest.md) |  | 

### Return type

[**FirewallVersion**](FirewallVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteFirewallVersion

> FirewallVersionMeta DeleteFirewallVersion(ctx, firewallId, versionId).Execute()

Delete a Firewall version



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
	firewallId := int64(789) // int64 | The ID of the Firewall resource.
	versionId := "versionId_example" // string | The identifier of the version.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallVersionsAPI.DeleteFirewallVersion(context.Background(), firewallId, versionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallVersionsAPI.DeleteFirewallVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteFirewallVersion`: FirewallVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `FirewallVersionsAPI.DeleteFirewallVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | The ID of the Firewall resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteFirewallVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**FirewallVersionMeta**](FirewallVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListFirewallVersions

> PaginatedFirewallVersionList ListFirewallVersions(ctx, firewallId).Page(page).PageSize(pageSize).Version(version).Execute()

List Firewall versions



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
	firewallId := int64(789) // int64 | The ID of the Firewall resource.
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	version := "version_example" // string | Narrow the list to one version. `latest`, in any case, answers the published version, or an empty list when none is published. Any other value matches a `version_id` and answers an empty list when none matches. An empty value is no filter. A resource that saves and builds in the same request (save and build) publishes no latest version, and `latest` on it answers 400 with code `10000`. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallVersionsAPI.ListFirewallVersions(context.Background(), firewallId).Page(page).PageSize(pageSize).Version(version).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallVersionsAPI.ListFirewallVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListFirewallVersions`: PaginatedFirewallVersionList
	fmt.Fprintf(os.Stdout, "Response from `FirewallVersionsAPI.ListFirewallVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | The ID of the Firewall resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListFirewallVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **version** | **string** | Narrow the list to one version. &#x60;latest&#x60;, in any case, answers the published version, or an empty list when none is published. Any other value matches a &#x60;version_id&#x60; and answers an empty list when none matches. An empty value is no filter. A resource that saves and builds in the same request (save and build) publishes no latest version, and &#x60;latest&#x60; on it answers 400 with code &#x60;10000&#x60;. | 

### Return type

[**PaginatedFirewallVersionList**](PaginatedFirewallVersionList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateFirewallVersion

> FirewallVersion PartialUpdateFirewallVersion(ctx, firewallId, versionId).PatchedFirewallRequest(patchedFirewallRequest).Execute()

Partially update a Firewall version



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
	firewallId := int64(789) // int64 | The ID of the Firewall resource.
	versionId := "versionId_example" // string | The identifier of the version.
	patchedFirewallRequest := *openapiclient.NewPatchedFirewallRequest() // PatchedFirewallRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallVersionsAPI.PartialUpdateFirewallVersion(context.Background(), firewallId, versionId).PatchedFirewallRequest(patchedFirewallRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallVersionsAPI.PartialUpdateFirewallVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateFirewallVersion`: FirewallVersion
	fmt.Fprintf(os.Stdout, "Response from `FirewallVersionsAPI.PartialUpdateFirewallVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | The ID of the Firewall resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateFirewallVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **patchedFirewallRequest** | [**PatchedFirewallRequest**](PatchedFirewallRequest.md) |  | 

### Return type

[**FirewallVersion**](FirewallVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveFirewallVersion

> FirewallVersion RetrieveFirewallVersion(ctx, firewallId, versionId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()

Retrieve a Firewall version



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
	firewallId := int64(789) // int64 | The ID of the Firewall resource.
	versionId := "versionId_example" // string | The identifier of the version.
	dependencies := true // bool | Include the resources this version references. (optional)
	dependencyStates := []string{"Inner_example"} // []string | Keep only the dependency versions in these states (comma-separated). Needs dependencies=true. Accepted states: `draft`, `queued`, `building`, `ready`, `error`, `canceled`, `archiving`, `archived`. An unknown state matches nothing, `deleting` and `deleted` match nothing because a dependency version in those states is never listed, and the match is case sensitive (`READY` matches nothing). (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallVersionsAPI.RetrieveFirewallVersion(context.Background(), firewallId, versionId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallVersionsAPI.RetrieveFirewallVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveFirewallVersion`: FirewallVersion
	fmt.Fprintf(os.Stdout, "Response from `FirewallVersionsAPI.RetrieveFirewallVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | The ID of the Firewall resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveFirewallVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **dependencies** | **bool** | Include the resources this version references. | 
 **dependencyStates** | **[]string** | Keep only the dependency versions in these states (comma-separated). Needs dependencies&#x3D;true. Accepted states: &#x60;draft&#x60;, &#x60;queued&#x60;, &#x60;building&#x60;, &#x60;ready&#x60;, &#x60;error&#x60;, &#x60;canceled&#x60;, &#x60;archiving&#x60;, &#x60;archived&#x60;. An unknown state matches nothing, &#x60;deleting&#x60; and &#x60;deleted&#x60; match nothing because a dependency version in those states is never listed, and the match is case sensitive (&#x60;READY&#x60; matches nothing). | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**FirewallVersion**](FirewallVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateFirewallVersion

> FirewallVersion UpdateFirewallVersion(ctx, firewallId, versionId).FirewallRequest(firewallRequest).Execute()

Update a Firewall version



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
	firewallId := int64(789) // int64 | The ID of the Firewall resource.
	versionId := "versionId_example" // string | The identifier of the version.
	firewallRequest := *openapiclient.NewFirewallRequest("Name_example") // FirewallRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallVersionsAPI.UpdateFirewallVersion(context.Background(), firewallId, versionId).FirewallRequest(firewallRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallVersionsAPI.UpdateFirewallVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateFirewallVersion`: FirewallVersion
	fmt.Fprintf(os.Stdout, "Response from `FirewallVersionsAPI.UpdateFirewallVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | The ID of the Firewall resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateFirewallVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **firewallRequest** | [**FirewallRequest**](FirewallRequest.md) |  | 

### Return type

[**FirewallVersion**](FirewallVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

