# \EnvironmentsAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ArchiveEnvironment**](EnvironmentsAPI.md#ArchiveEnvironment) | **Post** /environments/{environment_id}/archive | Archive an environment
[**CreateEnvironment**](EnvironmentsAPI.md#CreateEnvironment) | **Post** /environments | Create an Environment
[**DeleteEnvironment**](EnvironmentsAPI.md#DeleteEnvironment) | **Delete** /environments/{environment_id} | Delete an Environment
[**ListEnvironments**](EnvironmentsAPI.md#ListEnvironments) | **Get** /environments | List Environments
[**PartialUpdateEnvironment**](EnvironmentsAPI.md#PartialUpdateEnvironment) | **Patch** /environments/{environment_id} | Partially update an Environment
[**RetrieveEnvironment**](EnvironmentsAPI.md#RetrieveEnvironment) | **Get** /environments/{environment_id} | Retrieve details of an Environment
[**UpdateEnvironment**](EnvironmentsAPI.md#UpdateEnvironment) | **Put** /environments/{environment_id} | Update an Environment



## ArchiveEnvironment

> ArchiveEnvironmentResponse ArchiveEnvironment(ctx, environmentId).ArchiveEnvironmentRequest(archiveEnvironmentRequest).Execute()

Archive an environment



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
	environmentId := "environmentId_example" // string | A unique value identifying the environment.
	archiveEnvironmentRequest := *openapiclient.NewArchiveEnvironmentRequest("Reason_example") // ArchiveEnvironmentRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EnvironmentsAPI.ArchiveEnvironment(context.Background(), environmentId).ArchiveEnvironmentRequest(archiveEnvironmentRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EnvironmentsAPI.ArchiveEnvironment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ArchiveEnvironment`: ArchiveEnvironmentResponse
	fmt.Fprintf(os.Stdout, "Response from `EnvironmentsAPI.ArchiveEnvironment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**environmentId** | **string** | A unique value identifying the environment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiArchiveEnvironmentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **archiveEnvironmentRequest** | [**ArchiveEnvironmentRequest**](ArchiveEnvironmentRequest.md) |  | 

### Return type

[**ArchiveEnvironmentResponse**](ArchiveEnvironmentResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateEnvironment

> EnvironmentResponse CreateEnvironment(ctx).EnvironmentCreateRequest(environmentCreateRequest).Execute()

Create an Environment



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
	environmentCreateRequest := *openapiclient.NewEnvironmentCreateRequest("Name_example", "DeploymentPolicy_example") // EnvironmentCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EnvironmentsAPI.CreateEnvironment(context.Background()).EnvironmentCreateRequest(environmentCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EnvironmentsAPI.CreateEnvironment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateEnvironment`: EnvironmentResponse
	fmt.Fprintf(os.Stdout, "Response from `EnvironmentsAPI.CreateEnvironment`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateEnvironmentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **environmentCreateRequest** | [**EnvironmentCreateRequest**](EnvironmentCreateRequest.md) |  | 

### Return type

[**EnvironmentResponse**](EnvironmentResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteEnvironment

> DeleteResponse DeleteEnvironment(ctx, environmentId).Execute()

Delete an Environment



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
	environmentId := "environmentId_example" // string | A unique value identifying the environment.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EnvironmentsAPI.DeleteEnvironment(context.Background(), environmentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EnvironmentsAPI.DeleteEnvironment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteEnvironment`: DeleteResponse
	fmt.Fprintf(os.Stdout, "Response from `EnvironmentsAPI.DeleteEnvironment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**environmentId** | **string** | A unique value identifying the environment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteEnvironmentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DeleteResponse**](DeleteResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListEnvironments

> PaginatedEnvironmentList ListEnvironments(ctx).CreatedAtGte(createdAtGte).CreatedAtLte(createdAtLte).DeploymentPolicy(deploymentPolicy).Fields(fields).Id(id).IdIn(idIn).LastEditor(lastEditor).LastModifiedGte(lastModifiedGte).LastModifiedLte(lastModifiedLte).Name(name).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).State(state).StateIn(stateIn).Execute()

List Environments



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	createdAtGte := time.Now() // time.Time | Filter by creation date greater than or equal (ISO-8601) (optional)
	createdAtLte := time.Now() // time.Time | Filter by creation date less than or equal (ISO-8601) (optional)
	deploymentPolicy := "deploymentPolicy_example" // string | Filter by deployment policy (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	id := []string{"Inner_example"} // []string | Filter by environment ids (up to 100) (optional)
	idIn := []string{"Inner_example"} // []string | Filter by id (accepts comma-separated values). (optional)
	lastEditor := "lastEditor_example" // string | Filter by the email of the last editor (case-insensitive substring match) (optional)
	lastModifiedGte := time.Now() // time.Time | Filter by last-modified date greater than or equal (ISO-8601) (optional)
	lastModifiedLte := time.Now() // time.Time | Filter by last-modified date less than or equal (ISO-8601) (optional)
	name := "name_example" // string | Filter by environment name (case-insensitive substring match) (optional)
	ordering := "ordering_example" // string | Which field to use when ordering the results. (Valid fields: id, name, created_at, last_modified, version_state, deployment_policy, last_editor) (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	search := "search_example" // string | A search term to filter results. Searches across the following fields: name. (optional)
	state := []string{"Inner_example"} // []string | Filter by lifecycle state. `deleted` is rejected: a deleted environment never appears. (optional)
	stateIn := []string{"Inner_example"} // []string | Filter by state (accepts comma-separated values). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EnvironmentsAPI.ListEnvironments(context.Background()).CreatedAtGte(createdAtGte).CreatedAtLte(createdAtLte).DeploymentPolicy(deploymentPolicy).Fields(fields).Id(id).IdIn(idIn).LastEditor(lastEditor).LastModifiedGte(lastModifiedGte).LastModifiedLte(lastModifiedLte).Name(name).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).State(state).StateIn(stateIn).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EnvironmentsAPI.ListEnvironments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListEnvironments`: PaginatedEnvironmentList
	fmt.Fprintf(os.Stdout, "Response from `EnvironmentsAPI.ListEnvironments`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListEnvironmentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createdAtGte** | **time.Time** | Filter by creation date greater than or equal (ISO-8601) | 
 **createdAtLte** | **time.Time** | Filter by creation date less than or equal (ISO-8601) | 
 **deploymentPolicy** | **string** | Filter by deployment policy | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **id** | **[]string** | Filter by environment ids (up to 100) | 
 **idIn** | **[]string** | Filter by id (accepts comma-separated values). | 
 **lastEditor** | **string** | Filter by the email of the last editor (case-insensitive substring match) | 
 **lastModifiedGte** | **time.Time** | Filter by last-modified date greater than or equal (ISO-8601) | 
 **lastModifiedLte** | **time.Time** | Filter by last-modified date less than or equal (ISO-8601) | 
 **name** | **string** | Filter by environment name (case-insensitive substring match) | 
 **ordering** | **string** | Which field to use when ordering the results. (Valid fields: id, name, created_at, last_modified, version_state, deployment_policy, last_editor) | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **search** | **string** | A search term to filter results. Searches across the following fields: name. | 
 **state** | **[]string** | Filter by lifecycle state. &#x60;deleted&#x60; is rejected: a deleted environment never appears. | 
 **stateIn** | **[]string** | Filter by state (accepts comma-separated values). | 

### Return type

[**PaginatedEnvironmentList**](PaginatedEnvironmentList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateEnvironment

> EnvironmentResponse PartialUpdateEnvironment(ctx, environmentId).PatchedEnvironmentRequest(patchedEnvironmentRequest).Execute()

Partially update an Environment



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
	environmentId := "environmentId_example" // string | A unique value identifying the environment.
	patchedEnvironmentRequest := *openapiclient.NewPatchedEnvironmentRequest() // PatchedEnvironmentRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EnvironmentsAPI.PartialUpdateEnvironment(context.Background(), environmentId).PatchedEnvironmentRequest(patchedEnvironmentRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EnvironmentsAPI.PartialUpdateEnvironment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateEnvironment`: EnvironmentResponse
	fmt.Fprintf(os.Stdout, "Response from `EnvironmentsAPI.PartialUpdateEnvironment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**environmentId** | **string** | A unique value identifying the environment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateEnvironmentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **patchedEnvironmentRequest** | [**PatchedEnvironmentRequest**](PatchedEnvironmentRequest.md) |  | 

### Return type

[**EnvironmentResponse**](EnvironmentResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveEnvironment

> EnvironmentRetrieveResponse RetrieveEnvironment(ctx, environmentId).Fields(fields).Execute()

Retrieve details of an Environment



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
	environmentId := "environmentId_example" // string | A unique value identifying the environment.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EnvironmentsAPI.RetrieveEnvironment(context.Background(), environmentId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EnvironmentsAPI.RetrieveEnvironment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveEnvironment`: EnvironmentRetrieveResponse
	fmt.Fprintf(os.Stdout, "Response from `EnvironmentsAPI.RetrieveEnvironment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**environmentId** | **string** | A unique value identifying the environment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveEnvironmentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**EnvironmentRetrieveResponse**](EnvironmentRetrieveResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateEnvironment

> EnvironmentResponse UpdateEnvironment(ctx, environmentId).EnvironmentRequest(environmentRequest).Execute()

Update an Environment



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
	environmentId := "environmentId_example" // string | A unique value identifying the environment.
	environmentRequest := *openapiclient.NewEnvironmentRequest("Name_example", "Description_example", "LogVerbosity_example", "RobotsPolicy_example", *openapiclient.NewEnvironmentCreateRequestProtection(), "TODO") // EnvironmentRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EnvironmentsAPI.UpdateEnvironment(context.Background(), environmentId).EnvironmentRequest(environmentRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EnvironmentsAPI.UpdateEnvironment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateEnvironment`: EnvironmentResponse
	fmt.Fprintf(os.Stdout, "Response from `EnvironmentsAPI.UpdateEnvironment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**environmentId** | **string** | A unique value identifying the environment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateEnvironmentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **environmentRequest** | [**EnvironmentRequest**](EnvironmentRequest.md) |  | 

### Return type

[**EnvironmentResponse**](EnvironmentResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

