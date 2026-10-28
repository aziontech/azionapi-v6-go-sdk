# \ConnectorVersionsAPI

All URIs are relative to *https://api.azion.com/v6*

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

> ArchiveConnectorVersion(ctx, connectorId, versionId).VersionArchiveRequest(versionArchiveRequest).Execute()

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
	versionArchiveRequest := *openapiclient.NewVersionArchiveRequest() // VersionArchiveRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ConnectorVersionsAPI.ArchiveConnectorVersion(context.Background(), connectorId, versionId).VersionArchiveRequest(versionArchiveRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.ArchiveConnectorVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
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


 **versionArchiveRequest** | [**VersionArchiveRequest**](VersionArchiveRequest.md) |  | 

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


## BuildConnectorVersion

> BuildConnectorVersion(ctx, connectorId, versionId).VersionBuildRequest(versionBuildRequest).Execute()

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
	versionBuildRequest := *openapiclient.NewVersionBuildRequest() // VersionBuildRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ConnectorVersionsAPI.BuildConnectorVersion(context.Background(), connectorId, versionId).VersionBuildRequest(versionBuildRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.BuildConnectorVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
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


 **versionBuildRequest** | [**VersionBuildRequest**](VersionBuildRequest.md) |  | 

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


## CancelConnectorVersionBuild

> CancelConnectorVersionBuild(ctx, connectorId, versionId).VersionCancelRequest(versionCancelRequest).Execute()

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
	versionCancelRequest := *openapiclient.NewVersionCancelRequest() // VersionCancelRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ConnectorVersionsAPI.CancelConnectorVersionBuild(context.Background(), connectorId, versionId).VersionCancelRequest(versionCancelRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.CancelConnectorVersionBuild``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
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


 **versionCancelRequest** | [**VersionCancelRequest**](VersionCancelRequest.md) |  | 

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


## CreateConnectorVersion

> Connector CreateConnectorVersion(ctx, connectorId).VersionCreateRequest(versionCreateRequest).Execute()

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
	versionCreateRequest := *openapiclient.NewVersionCreateRequest() // VersionCreateRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConnectorVersionsAPI.CreateConnectorVersion(context.Background(), connectorId).VersionCreateRequest(versionCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.CreateConnectorVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateConnectorVersion`: Connector
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

 **versionCreateRequest** | [**VersionCreateRequest**](VersionCreateRequest.md) |  | 

### Return type

[**Connector**](Connector.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteConnectorVersion

> DeleteConnectorVersion(ctx, connectorId, versionId).Execute()

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
	r, err := apiClient.ConnectorVersionsAPI.DeleteConnectorVersion(context.Background(), connectorId, versionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.DeleteConnectorVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
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

 (empty response body)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListConnectorVersions

> PaginatedConnectorList ListConnectorVersions(ctx, connectorId).Fields(fields).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()

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
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	ordering := "ordering_example" // string | Which field to use when ordering the results. (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	search := "search_example" // string | A search term. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConnectorVersionsAPI.ListConnectorVersions(context.Background(), connectorId).Fields(fields).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.ListConnectorVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListConnectorVersions`: PaginatedConnectorList
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

 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **ordering** | **string** | Which field to use when ordering the results. | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **search** | **string** | A search term. | 

### Return type

[**PaginatedConnectorList**](PaginatedConnectorList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateConnectorVersion

> Connector PartialUpdateConnectorVersion(ctx, connectorId, versionId).PatchedConnectorRequest(patchedConnectorRequest).Execute()

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
	// response from `PartialUpdateConnectorVersion`: Connector
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

[**Connector**](Connector.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveConnectorVersion

> Connector RetrieveConnectorVersion(ctx, connectorId, versionId).Fields(fields).Execute()

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
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ConnectorVersionsAPI.RetrieveConnectorVersion(context.Background(), connectorId, versionId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ConnectorVersionsAPI.RetrieveConnectorVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveConnectorVersion`: Connector
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


 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**Connector**](Connector.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateConnectorVersion

> Connector UpdateConnectorVersion(ctx, connectorId, versionId).ConnectorRequest(connectorRequest).Execute()

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
	// response from `UpdateConnectorVersion`: Connector
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

[**Connector**](Connector.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

