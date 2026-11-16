# \NetworkListVersionsAPI

All URIs are relative to *https://stage-api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ArchiveNetworkListVersion**](NetworkListVersionsAPI.md#ArchiveNetworkListVersion) | **Post** /workspace/network_lists/{network_list_id}/versions/{version_id}/archive | Archive a Network List version
[**BuildNetworkListVersion**](NetworkListVersionsAPI.md#BuildNetworkListVersion) | **Post** /workspace/network_lists/{network_list_id}/versions/{version_id}/build | Build a Network List version
[**CancelNetworkListVersionBuild**](NetworkListVersionsAPI.md#CancelNetworkListVersionBuild) | **Post** /workspace/network_lists/{network_list_id}/versions/{version_id}/cancel | Cancel a Network List version build
[**CreateNetworkListVersion**](NetworkListVersionsAPI.md#CreateNetworkListVersion) | **Post** /workspace/network_lists/{network_list_id}/versions | Create a new Network List version
[**DeleteNetworkListVersion**](NetworkListVersionsAPI.md#DeleteNetworkListVersion) | **Delete** /workspace/network_lists/{network_list_id}/versions/{version_id} | Delete a Network List version
[**ListNetworkListVersions**](NetworkListVersionsAPI.md#ListNetworkListVersions) | **Get** /workspace/network_lists/{network_list_id}/versions | List Network List versions
[**PartialUpdateNetworkListVersion**](NetworkListVersionsAPI.md#PartialUpdateNetworkListVersion) | **Patch** /workspace/network_lists/{network_list_id}/versions/{version_id} | Partially update a Network List version
[**RetrieveNetworkListVersion**](NetworkListVersionsAPI.md#RetrieveNetworkListVersion) | **Get** /workspace/network_lists/{network_list_id}/versions/{version_id} | Retrieve a Network List version
[**UpdateNetworkListVersion**](NetworkListVersionsAPI.md#UpdateNetworkListVersion) | **Put** /workspace/network_lists/{network_list_id}/versions/{version_id} | Update a Network List version



## ArchiveNetworkListVersion

> NetworkListVersionMeta ArchiveNetworkListVersion(ctx, networkListId, versionId).NetworkListVersionArchiveRequest(networkListVersionArchiveRequest).Execute()

Archive a Network List version



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
	networkListId := int64(789) // int64 | The ID of the Network List resource.
	versionId := "versionId_example" // string | The identifier of the version.
	networkListVersionArchiveRequest := *openapiclient.NewNetworkListVersionArchiveRequest() // NetworkListVersionArchiveRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NetworkListVersionsAPI.ArchiveNetworkListVersion(context.Background(), networkListId, versionId).NetworkListVersionArchiveRequest(networkListVersionArchiveRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NetworkListVersionsAPI.ArchiveNetworkListVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ArchiveNetworkListVersion`: NetworkListVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `NetworkListVersionsAPI.ArchiveNetworkListVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**networkListId** | **int64** | The ID of the Network List resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiArchiveNetworkListVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **networkListVersionArchiveRequest** | [**NetworkListVersionArchiveRequest**](NetworkListVersionArchiveRequest.md) |  | 

### Return type

[**NetworkListVersionMeta**](NetworkListVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BuildNetworkListVersion

> NetworkListVersionMeta BuildNetworkListVersion(ctx, networkListId, versionId).NetworkListVersionBuildRequest(networkListVersionBuildRequest).Execute()

Build a Network List version



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
	networkListId := int64(789) // int64 | The ID of the Network List resource.
	versionId := "versionId_example" // string | The identifier of the version.
	networkListVersionBuildRequest := *openapiclient.NewNetworkListVersionBuildRequest() // NetworkListVersionBuildRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NetworkListVersionsAPI.BuildNetworkListVersion(context.Background(), networkListId, versionId).NetworkListVersionBuildRequest(networkListVersionBuildRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NetworkListVersionsAPI.BuildNetworkListVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BuildNetworkListVersion`: NetworkListVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `NetworkListVersionsAPI.BuildNetworkListVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**networkListId** | **int64** | The ID of the Network List resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBuildNetworkListVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **networkListVersionBuildRequest** | [**NetworkListVersionBuildRequest**](NetworkListVersionBuildRequest.md) |  | 

### Return type

[**NetworkListVersionMeta**](NetworkListVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelNetworkListVersionBuild

> NetworkListVersionMeta CancelNetworkListVersionBuild(ctx, networkListId, versionId).NetworkListVersionCancelRequest(networkListVersionCancelRequest).Execute()

Cancel a Network List version build



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
	networkListId := int64(789) // int64 | The ID of the Network List resource.
	versionId := "versionId_example" // string | The identifier of the version.
	networkListVersionCancelRequest := *openapiclient.NewNetworkListVersionCancelRequest() // NetworkListVersionCancelRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NetworkListVersionsAPI.CancelNetworkListVersionBuild(context.Background(), networkListId, versionId).NetworkListVersionCancelRequest(networkListVersionCancelRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NetworkListVersionsAPI.CancelNetworkListVersionBuild``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelNetworkListVersionBuild`: NetworkListVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `NetworkListVersionsAPI.CancelNetworkListVersionBuild`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**networkListId** | **int64** | The ID of the Network List resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelNetworkListVersionBuildRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **networkListVersionCancelRequest** | [**NetworkListVersionCancelRequest**](NetworkListVersionCancelRequest.md) |  | 

### Return type

[**NetworkListVersionMeta**](NetworkListVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateNetworkListVersion

> NetworkListVersion CreateNetworkListVersion(ctx, networkListId).NetworkListVersionCreateRequest(networkListVersionCreateRequest).Execute()

Create a new Network List version



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
	networkListId := int64(789) // int64 | The ID of the Network List resource.
	networkListVersionCreateRequest := *openapiclient.NewNetworkListVersionCreateRequest() // NetworkListVersionCreateRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NetworkListVersionsAPI.CreateNetworkListVersion(context.Background(), networkListId).NetworkListVersionCreateRequest(networkListVersionCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NetworkListVersionsAPI.CreateNetworkListVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateNetworkListVersion`: NetworkListVersion
	fmt.Fprintf(os.Stdout, "Response from `NetworkListVersionsAPI.CreateNetworkListVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**networkListId** | **int64** | The ID of the Network List resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateNetworkListVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **networkListVersionCreateRequest** | [**NetworkListVersionCreateRequest**](NetworkListVersionCreateRequest.md) |  | 

### Return type

[**NetworkListVersion**](NetworkListVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteNetworkListVersion

> NetworkListVersionMeta DeleteNetworkListVersion(ctx, networkListId, versionId).Execute()

Delete a Network List version



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
	networkListId := int64(789) // int64 | The ID of the Network List resource.
	versionId := "versionId_example" // string | The identifier of the version.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NetworkListVersionsAPI.DeleteNetworkListVersion(context.Background(), networkListId, versionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NetworkListVersionsAPI.DeleteNetworkListVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteNetworkListVersion`: NetworkListVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `NetworkListVersionsAPI.DeleteNetworkListVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**networkListId** | **int64** | The ID of the Network List resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteNetworkListVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**NetworkListVersionMeta**](NetworkListVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListNetworkListVersions

> PaginatedNetworkListVersionList ListNetworkListVersions(ctx, networkListId).Page(page).PageSize(pageSize).Version(version).Execute()

List Network List versions



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
	networkListId := int64(789) // int64 | The ID of the Network List resource.
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	version := "version_example" // string | Narrow the list to one version. `latest`, in any case, answers the published version, or an empty list when none is published. Any other value matches a `version_id` and answers an empty list when none matches. An empty value is no filter. A resource that saves and builds in the same request (save and build) publishes no latest version, and `latest` on it answers 400 with code `10000`. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NetworkListVersionsAPI.ListNetworkListVersions(context.Background(), networkListId).Page(page).PageSize(pageSize).Version(version).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NetworkListVersionsAPI.ListNetworkListVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListNetworkListVersions`: PaginatedNetworkListVersionList
	fmt.Fprintf(os.Stdout, "Response from `NetworkListVersionsAPI.ListNetworkListVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**networkListId** | **int64** | The ID of the Network List resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListNetworkListVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **version** | **string** | Narrow the list to one version. &#x60;latest&#x60;, in any case, answers the published version, or an empty list when none is published. Any other value matches a &#x60;version_id&#x60; and answers an empty list when none matches. An empty value is no filter. A resource that saves and builds in the same request (save and build) publishes no latest version, and &#x60;latest&#x60; on it answers 400 with code &#x60;10000&#x60;. | 

### Return type

[**PaginatedNetworkListVersionList**](PaginatedNetworkListVersionList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateNetworkListVersion

> NetworkListVersion PartialUpdateNetworkListVersion(ctx, networkListId, versionId).PatchedNetworkListRequest(patchedNetworkListRequest).Execute()

Partially update a Network List version



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
	networkListId := int64(789) // int64 | The ID of the Network List resource.
	versionId := "versionId_example" // string | The identifier of the version.
	patchedNetworkListRequest := *openapiclient.NewPatchedNetworkListRequest() // PatchedNetworkListRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NetworkListVersionsAPI.PartialUpdateNetworkListVersion(context.Background(), networkListId, versionId).PatchedNetworkListRequest(patchedNetworkListRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NetworkListVersionsAPI.PartialUpdateNetworkListVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateNetworkListVersion`: NetworkListVersion
	fmt.Fprintf(os.Stdout, "Response from `NetworkListVersionsAPI.PartialUpdateNetworkListVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**networkListId** | **int64** | The ID of the Network List resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateNetworkListVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **patchedNetworkListRequest** | [**PatchedNetworkListRequest**](PatchedNetworkListRequest.md) |  | 

### Return type

[**NetworkListVersion**](NetworkListVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveNetworkListVersion

> NetworkListVersion RetrieveNetworkListVersion(ctx, networkListId, versionId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Ipv4(ipv4).Ipv6(ipv6).Execute()

Retrieve a Network List version



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
	networkListId := int64(789) // int64 | The ID of the Network List resource.
	versionId := "versionId_example" // string | The identifier of the version.
	dependencies := true // bool | Include the resources this version references. (optional)
	dependencyStates := []string{"Inner_example"} // []string | Keep only the dependency versions in these states (comma-separated). Needs dependencies=true. Accepted states: `draft`, `queued`, `building`, `ready`, `error`, `canceled`, `archiving`, `archived`. An unknown state matches nothing, `deleting` and `deleted` match nothing because a dependency version in those states is never listed, and the match is case sensitive (`READY` matches nothing). (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	ipv4 := true // bool | Keep the IPv4 entries in `items`. Only applicable for network lists of type 'ip_cidr'. Only `true` (case-insensitive) turns a flag on. When only one of ipv4 and ipv6 is sent, the other takes the opposite value. When neither is sent, both are on. When both are off, `items` is empty. (optional)
	ipv6 := true // bool | Keep the IPv6 entries in `items`. Only applicable for network lists of type 'ip_cidr'. Only `true` (case-insensitive) turns a flag on. When only one of ipv4 and ipv6 is sent, the other takes the opposite value. When neither is sent, both are on. When both are off, `items` is empty. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NetworkListVersionsAPI.RetrieveNetworkListVersion(context.Background(), networkListId, versionId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Ipv4(ipv4).Ipv6(ipv6).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NetworkListVersionsAPI.RetrieveNetworkListVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveNetworkListVersion`: NetworkListVersion
	fmt.Fprintf(os.Stdout, "Response from `NetworkListVersionsAPI.RetrieveNetworkListVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**networkListId** | **int64** | The ID of the Network List resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveNetworkListVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **dependencies** | **bool** | Include the resources this version references. | 
 **dependencyStates** | **[]string** | Keep only the dependency versions in these states (comma-separated). Needs dependencies&#x3D;true. Accepted states: &#x60;draft&#x60;, &#x60;queued&#x60;, &#x60;building&#x60;, &#x60;ready&#x60;, &#x60;error&#x60;, &#x60;canceled&#x60;, &#x60;archiving&#x60;, &#x60;archived&#x60;. An unknown state matches nothing, &#x60;deleting&#x60; and &#x60;deleted&#x60; match nothing because a dependency version in those states is never listed, and the match is case sensitive (&#x60;READY&#x60; matches nothing). | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **ipv4** | **bool** | Keep the IPv4 entries in &#x60;items&#x60;. Only applicable for network lists of type &#39;ip_cidr&#39;. Only &#x60;true&#x60; (case-insensitive) turns a flag on. When only one of ipv4 and ipv6 is sent, the other takes the opposite value. When neither is sent, both are on. When both are off, &#x60;items&#x60; is empty. | 
 **ipv6** | **bool** | Keep the IPv6 entries in &#x60;items&#x60;. Only applicable for network lists of type &#39;ip_cidr&#39;. Only &#x60;true&#x60; (case-insensitive) turns a flag on. When only one of ipv4 and ipv6 is sent, the other takes the opposite value. When neither is sent, both are on. When both are off, &#x60;items&#x60; is empty. | 

### Return type

[**NetworkListVersion**](NetworkListVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateNetworkListVersion

> NetworkListVersion UpdateNetworkListVersion(ctx, networkListId, versionId).NetworkListRequest(networkListRequest).Execute()

Update a Network List version



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
	networkListId := int64(789) // int64 | The ID of the Network List resource.
	versionId := "versionId_example" // string | The identifier of the version.
	networkListRequest := *openapiclient.NewNetworkListRequest("Name_example", "Type_example", []string{"Items_example"}) // NetworkListRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.NetworkListVersionsAPI.UpdateNetworkListVersion(context.Background(), networkListId, versionId).NetworkListRequest(networkListRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `NetworkListVersionsAPI.UpdateNetworkListVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateNetworkListVersion`: NetworkListVersion
	fmt.Fprintf(os.Stdout, "Response from `NetworkListVersionsAPI.UpdateNetworkListVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**networkListId** | **int64** | The ID of the Network List resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateNetworkListVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **networkListRequest** | [**NetworkListRequest**](NetworkListRequest.md) |  | 

### Return type

[**NetworkListVersion**](NetworkListVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

