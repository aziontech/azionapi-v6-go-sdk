# \ConnectorVersionsAPI

All URIs are relative to *https://stage-api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ArchiveConnectorVersion**](ConnectorVersionsAPI.md#ArchiveConnectorVersion) | **Post** /workspace/connectors/{connector_id}/versions/{version_id}/archive | Archive a Connector version
[**BuildConnectorVersion**](ConnectorVersionsAPI.md#BuildConnectorVersion) | **Post** /workspace/connectors/{connector_id}/versions/{version_id}/build | Build a Connector version
[**CancelConnectorVersionBuild**](ConnectorVersionsAPI.md#CancelConnectorVersionBuild) | **Post** /workspace/connectors/{connector_id}/versions/{version_id}/cancel | Cancel a Connector version build
[**CreateConnectorVersion**](ConnectorVersionsAPI.md#CreateConnectorVersion) | **Post** /workspace/connectors/{connector_id}/versions | Create a new Connector version
[**DeleteConnectorVersion**](ConnectorVersionsAPI.md#DeleteConnectorVersion) | **Delete** /workspace/connectors/{connector_id}/versions/{version_id} | Delete a Connector version
[**ListConnectorVersions**](ConnectorVersionsAPI.md#ListConnectorVersions) | **Get** /workspace/connectors/{connector_id}/versions | List Connector versions
[**PartialUpdateConnectorVersion**](ConnectorVersionsAPI.md#PartialUpdateConnectorVersion) | **Patch** /workspace/connectors/{connector_id}/versions/{version_id} | Partially update a Connector version
[**RetrieveConnectorVersion**](ConnectorVersionsAPI.md#RetrieveConnectorVersion) | **Get** /workspace/connectors/{connector_id}/versions/{version_id} | Retrieve a Connector version
[**UpdateConnectorVersion**](ConnectorVersionsAPI.md#UpdateConnectorVersion) | **Put** /workspace/connectors/{connector_id}/versions/{version_id} | Update a Connector version



## ArchiveConnectorVersion

> ConnectorVersionMeta ArchiveConnectorVersion(ctx, connectorId, versionId).ConnectorVersionArchiveRequest(connectorVersionArchiveRequest).Execute()

Archive a Connector version



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
	connectorId := int64(789) // int64 | The ID of the Connector resource.
	versionId := "versionId_example" // string | The identifier of the version.
	connectorVersionArchiveRequest := *openapiclient.NewConnectorVersionArchiveRequest() // ConnectorVersionArchiveRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConnectorVersionsAPI.ArchiveConnectorVersion(context.Background(), connectorId, versionId).ConnectorVersionArchiveRequest(connectorVersionArchiveRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.ArchiveConnectorVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ArchiveConnectorVersion`: ConnectorVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `ConnectorVersionsAPI.ArchiveConnectorVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**connectorId** | **int64** | The ID of the Connector resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiArchiveConnectorVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **connectorVersionArchiveRequest** | [**ConnectorVersionArchiveRequest**](ConnectorVersionArchiveRequest.md) |  | 

### Return type

[**ConnectorVersionMeta**](ConnectorVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BuildConnectorVersion

> ConnectorVersionMeta BuildConnectorVersion(ctx, connectorId, versionId).ConnectorVersionBuildRequest(connectorVersionBuildRequest).Execute()

Build a Connector version



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
	connectorId := int64(789) // int64 | The ID of the Connector resource.
	versionId := "versionId_example" // string | The identifier of the version.
	connectorVersionBuildRequest := *openapiclient.NewConnectorVersionBuildRequest() // ConnectorVersionBuildRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConnectorVersionsAPI.BuildConnectorVersion(context.Background(), connectorId, versionId).ConnectorVersionBuildRequest(connectorVersionBuildRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.BuildConnectorVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BuildConnectorVersion`: ConnectorVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `ConnectorVersionsAPI.BuildConnectorVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**connectorId** | **int64** | The ID of the Connector resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiBuildConnectorVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **connectorVersionBuildRequest** | [**ConnectorVersionBuildRequest**](ConnectorVersionBuildRequest.md) |  | 

### Return type

[**ConnectorVersionMeta**](ConnectorVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CancelConnectorVersionBuild

> ConnectorVersionMeta CancelConnectorVersionBuild(ctx, connectorId, versionId).ConnectorVersionCancelRequest(connectorVersionCancelRequest).Execute()

Cancel a Connector version build



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
	connectorId := int64(789) // int64 | The ID of the Connector resource.
	versionId := "versionId_example" // string | The identifier of the version.
	connectorVersionCancelRequest := *openapiclient.NewConnectorVersionCancelRequest() // ConnectorVersionCancelRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConnectorVersionsAPI.CancelConnectorVersionBuild(context.Background(), connectorId, versionId).ConnectorVersionCancelRequest(connectorVersionCancelRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.CancelConnectorVersionBuild``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CancelConnectorVersionBuild`: ConnectorVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `ConnectorVersionsAPI.CancelConnectorVersionBuild`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**connectorId** | **int64** | The ID of the Connector resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCancelConnectorVersionBuildRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **connectorVersionCancelRequest** | [**ConnectorVersionCancelRequest**](ConnectorVersionCancelRequest.md) |  | 

### Return type

[**ConnectorVersionMeta**](ConnectorVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateConnectorVersion

> ConnectorVersion CreateConnectorVersion(ctx, connectorId).ConnectorVersionCreateRequest(connectorVersionCreateRequest).Execute()

Create a new Connector version



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
	connectorId := int64(789) // int64 | The ID of the Connector resource.
	connectorVersionCreateRequest := *openapiclient.NewConnectorVersionCreateRequest() // ConnectorVersionCreateRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConnectorVersionsAPI.CreateConnectorVersion(context.Background(), connectorId).ConnectorVersionCreateRequest(connectorVersionCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.CreateConnectorVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateConnectorVersion`: ConnectorVersion
	fmt.Fprintf(os.Stdout, "Response from `ConnectorVersionsAPI.CreateConnectorVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**connectorId** | **int64** | The ID of the Connector resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateConnectorVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **connectorVersionCreateRequest** | [**ConnectorVersionCreateRequest**](ConnectorVersionCreateRequest.md) |  | 

### Return type

[**ConnectorVersion**](ConnectorVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteConnectorVersion

> ConnectorVersionMeta DeleteConnectorVersion(ctx, connectorId, versionId).Execute()

Delete a Connector version



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
	connectorId := int64(789) // int64 | The ID of the Connector resource.
	versionId := "versionId_example" // string | The identifier of the version.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConnectorVersionsAPI.DeleteConnectorVersion(context.Background(), connectorId, versionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.DeleteConnectorVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteConnectorVersion`: ConnectorVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `ConnectorVersionsAPI.DeleteConnectorVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**connectorId** | **int64** | The ID of the Connector resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteConnectorVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ConnectorVersionMeta**](ConnectorVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListConnectorVersions

> PaginatedConnectorVersionList ListConnectorVersions(ctx, connectorId).Page(page).PageSize(pageSize).Execute()

List Connector versions



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
	connectorId := int64(789) // int64 | The ID of the Connector resource.
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConnectorVersionsAPI.ListConnectorVersions(context.Background(), connectorId).Page(page).PageSize(pageSize).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.ListConnectorVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListConnectorVersions`: PaginatedConnectorVersionList
	fmt.Fprintf(os.Stdout, "Response from `ConnectorVersionsAPI.ListConnectorVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**connectorId** | **int64** | The ID of the Connector resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListConnectorVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 

### Return type

[**PaginatedConnectorVersionList**](PaginatedConnectorVersionList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateConnectorVersion

> ConnectorVersion PartialUpdateConnectorVersion(ctx, connectorId, versionId).PatchedConnectorRequest(patchedConnectorRequest).Execute()

Partially update a Connector version



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
	connectorId := int64(789) // int64 | The ID of the Connector resource.
	versionId := "versionId_example" // string | The identifier of the version.
	patchedConnectorRequest := openapiclient.PatchedConnectorRequest{PatchedConnectorHTTPRequest: openapiclient.NewPatchedConnectorHTTPRequest("Type_example")} // PatchedConnectorRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConnectorVersionsAPI.PartialUpdateConnectorVersion(context.Background(), connectorId, versionId).PatchedConnectorRequest(patchedConnectorRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.PartialUpdateConnectorVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateConnectorVersion`: ConnectorVersion
	fmt.Fprintf(os.Stdout, "Response from `ConnectorVersionsAPI.PartialUpdateConnectorVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**connectorId** | **int64** | The ID of the Connector resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateConnectorVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **patchedConnectorRequest** | [**PatchedConnectorRequest**](PatchedConnectorRequest.md) |  | 

### Return type

[**ConnectorVersion**](ConnectorVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveConnectorVersion

> ConnectorVersion RetrieveConnectorVersion(ctx, connectorId, versionId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()

Retrieve a Connector version



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
	connectorId := int64(789) // int64 | The ID of the Connector resource.
	versionId := "versionId_example" // string | The identifier of the version.
	dependencies := true // bool | Include the resources this version references. (optional)
	dependencyStates := []string{"Inner_example"} // []string | Keep only the dependency versions in these states (comma-separated). Needs dependencies=true. (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConnectorVersionsAPI.RetrieveConnectorVersion(context.Background(), connectorId, versionId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.RetrieveConnectorVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveConnectorVersion`: ConnectorVersion
	fmt.Fprintf(os.Stdout, "Response from `ConnectorVersionsAPI.RetrieveConnectorVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**connectorId** | **int64** | The ID of the Connector resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveConnectorVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **dependencies** | **bool** | Include the resources this version references. | 
 **dependencyStates** | **[]string** | Keep only the dependency versions in these states (comma-separated). Needs dependencies&#x3D;true. | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**ConnectorVersion**](ConnectorVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateConnectorVersion

> ConnectorVersion UpdateConnectorVersion(ctx, connectorId, versionId).ConnectorRequest(connectorRequest).Execute()

Update a Connector version



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
	connectorId := int64(789) // int64 | The ID of the Connector resource.
	versionId := "versionId_example" // string | The identifier of the version.
	connectorRequest := openapiclient.ConnectorRequest{ConnectorHTTPRequest: openapiclient.NewConnectorHTTPRequest("Name_example", "Type_example", *openapiclient.NewConnectorHTTPAttributesRequest([]openapiclient.AddressRequest{*openapiclient.NewAddressRequest("Address_example")}))} // ConnectorRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConnectorVersionsAPI.UpdateConnectorVersion(context.Background(), connectorId, versionId).ConnectorRequest(connectorRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.UpdateConnectorVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateConnectorVersion`: ConnectorVersion
	fmt.Fprintf(os.Stdout, "Response from `ConnectorVersionsAPI.UpdateConnectorVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**connectorId** | **int64** | The ID of the Connector resource. | 
**versionId** | **string** | The identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateConnectorVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **connectorRequest** | [**ConnectorRequest**](ConnectorRequest.md) |  | 

### Return type

[**ConnectorVersion**](ConnectorVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

