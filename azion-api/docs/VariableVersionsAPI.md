# \VariableVersionsAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListVariableVersions**](VariableVersionsAPI.md#ListVariableVersions) | **Get** /variables/{variable_id}/versions | List Variable Versions
[**RetrieveVariableVersion**](VariableVersionsAPI.md#RetrieveVariableVersion) | **Get** /variables/{variable_id}/versions/{id} | Retrieve details of a Variable Version
[**RevertVariableVersion**](VariableVersionsAPI.md#RevertVariableVersion) | **Post** /variables/{variable_id}/revert/{id} | Revert to a Variable Version



## ListVariableVersions

> PaginatedVariableVersionListItemList ListVariableVersions(ctx, variableId).Page(page).PageSize(pageSize).Execute()

List Variable Versions



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
	variableId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | A unique value identifying the variable.
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VariableVersionsAPI.ListVariableVersions(context.Background(), variableId).Page(page).PageSize(pageSize).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VariableVersionsAPI.ListVariableVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListVariableVersions`: PaginatedVariableVersionListItemList
	fmt.Fprintf(os.Stdout, "Response from `VariableVersionsAPI.ListVariableVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**variableId** | **string** | A unique value identifying the variable. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListVariableVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 

### Return type

[**PaginatedVariableVersionListItemList**](PaginatedVariableVersionListItemList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveVariableVersion

> VariableVersionListItem RetrieveVariableVersion(ctx, id, variableId).Execute()

Retrieve details of a Variable Version



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
	id := "id_example" // string | A unique value identifying the variable version.
	variableId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | A unique value identifying the variable.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VariableVersionsAPI.RetrieveVariableVersion(context.Background(), id, variableId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VariableVersionsAPI.RetrieveVariableVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveVariableVersion`: VariableVersionListItem
	fmt.Fprintf(os.Stdout, "Response from `VariableVersionsAPI.RetrieveVariableVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | A unique value identifying the variable version. | 
**variableId** | **string** | A unique value identifying the variable. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveVariableVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**VariableVersionListItem**](VariableVersionListItem.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RevertVariableVersion

> VariableVersionListItem RevertVariableVersion(ctx, id, variableId).Execute()

Revert to a Variable Version



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
	id := "id_example" // string | A unique value identifying the variable version.
	variableId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | A unique value identifying the variable.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.VariableVersionsAPI.RevertVariableVersion(context.Background(), id, variableId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `VariableVersionsAPI.RevertVariableVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RevertVariableVersion`: VariableVersionListItem
	fmt.Fprintf(os.Stdout, "Response from `VariableVersionsAPI.RevertVariableVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | A unique value identifying the variable version. | 
**variableId** | **string** | A unique value identifying the variable. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRevertVariableVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**VariableVersionListItem**](VariableVersionListItem.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

