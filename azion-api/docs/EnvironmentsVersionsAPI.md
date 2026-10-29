# \EnvironmentsVersionsAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListEnvironmentVersions**](EnvironmentsVersionsAPI.md#ListEnvironmentVersions) | **Get** /environments/{environment_id}/versions | List environment versions
[**RetrieveEnvironmentVersion**](EnvironmentsVersionsAPI.md#RetrieveEnvironmentVersion) | **Get** /environments/{environment_id}/versions/{version_id} | Retrieve an environment version
[**RevertEnvironmentVersion**](EnvironmentsVersionsAPI.md#RevertEnvironmentVersion) | **Post** /environments/{environment_id}/versions/{version_id}/revert | Revert to an environment version



## ListEnvironmentVersions

> PaginatedEnvironmentVersionList ListEnvironmentVersions(ctx, environmentId).CreatedAtGte(createdAtGte).CreatedAtLte(createdAtLte).Description(description).Fields(fields).LastEditor(lastEditor).Ordering(ordering).Page(page).PageSize(pageSize).ReadyAtGte(readyAtGte).ReadyAtLte(readyAtLte).Search(search).Version(version).VersionGte(versionGte).VersionLte(versionLte).VersionState(versionState).VersionStateIn(versionStateIn).Execute()

List environment versions



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
	environmentId := "environmentId_example" // string | A unique value identifying the environment.
	createdAtGte := time.Now() // time.Time | Filter by creation date (greater than or equal). (optional)
	createdAtLte := time.Now() // time.Time | Filter by creation date (less than or equal). (optional)
	description := "description_example" // string | Filter by description (case-insensitive, partial match). (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	lastEditor := "lastEditor_example" // string | Filter by last editor (case-insensitive, partial match). (optional)
	ordering := "ordering_example" // string | Which field to use when ordering the results. (Valid fields: version, version_state, created_at, ready_at, last_editor) (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	readyAtGte := time.Now() // time.Time | Filter by ready date (greater than or equal). (optional)
	readyAtLte := time.Now() // time.Time | Filter by ready date (less than or equal). (optional)
	search := "search_example" // string | A search term to filter results. Searches across the following fields: description, last_editor. (optional)
	version := int32(56) // int32 | Filter by version. (optional)
	versionGte := int32(56) // int32 | Filter by version (greater than or equal). (optional)
	versionLte := int32(56) // int32 | Filter by version (less than or equal). (optional)
	versionState := []string{"Inner_example"} // []string | Filter by version state (accepts comma-separated values). (optional)
	versionStateIn := []string{"Inner_example"} // []string | Filter by version_state (accepts comma-separated values). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EnvironmentsVersionsAPI.ListEnvironmentVersions(context.Background(), environmentId).CreatedAtGte(createdAtGte).CreatedAtLte(createdAtLte).Description(description).Fields(fields).LastEditor(lastEditor).Ordering(ordering).Page(page).PageSize(pageSize).ReadyAtGte(readyAtGte).ReadyAtLte(readyAtLte).Search(search).Version(version).VersionGte(versionGte).VersionLte(versionLte).VersionState(versionState).VersionStateIn(versionStateIn).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EnvironmentsVersionsAPI.ListEnvironmentVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListEnvironmentVersions`: PaginatedEnvironmentVersionList
	fmt.Fprintf(os.Stdout, "Response from `EnvironmentsVersionsAPI.ListEnvironmentVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**environmentId** | **string** | A unique value identifying the environment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListEnvironmentVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createdAtGte** | **time.Time** | Filter by creation date (greater than or equal). | 
 **createdAtLte** | **time.Time** | Filter by creation date (less than or equal). | 
 **description** | **string** | Filter by description (case-insensitive, partial match). | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **lastEditor** | **string** | Filter by last editor (case-insensitive, partial match). | 
 **ordering** | **string** | Which field to use when ordering the results. (Valid fields: version, version_state, created_at, ready_at, last_editor) | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **readyAtGte** | **time.Time** | Filter by ready date (greater than or equal). | 
 **readyAtLte** | **time.Time** | Filter by ready date (less than or equal). | 
 **search** | **string** | A search term to filter results. Searches across the following fields: description, last_editor. | 
 **version** | **int32** | Filter by version. | 
 **versionGte** | **int32** | Filter by version (greater than or equal). | 
 **versionLte** | **int32** | Filter by version (less than or equal). | 
 **versionState** | **[]string** | Filter by version state (accepts comma-separated values). | 
 **versionStateIn** | **[]string** | Filter by version_state (accepts comma-separated values). | 

### Return type

[**PaginatedEnvironmentVersionList**](PaginatedEnvironmentVersionList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveEnvironmentVersion

> EnvironmentVersion RetrieveEnvironmentVersion(ctx, environmentId, versionId).Fields(fields).Execute()

Retrieve an environment version



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
	versionId := "versionId_example" // string | A unique value identifying the version.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EnvironmentsVersionsAPI.RetrieveEnvironmentVersion(context.Background(), environmentId, versionId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EnvironmentsVersionsAPI.RetrieveEnvironmentVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveEnvironmentVersion`: EnvironmentVersion
	fmt.Fprintf(os.Stdout, "Response from `EnvironmentsVersionsAPI.RetrieveEnvironmentVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**environmentId** | **string** | A unique value identifying the environment. | 
**versionId** | **string** | A unique value identifying the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveEnvironmentVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**EnvironmentVersion**](EnvironmentVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RevertEnvironmentVersion

> EnvironmentVersionMeta RevertEnvironmentVersion(ctx, environmentId, versionId).EnvironmentVersionRevertRequest(environmentVersionRevertRequest).Execute()

Revert to an environment version



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
	versionId := "versionId_example" // string | A unique value identifying the version.
	environmentVersionRevertRequest := *openapiclient.NewEnvironmentVersionRevertRequest() // EnvironmentVersionRevertRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EnvironmentsVersionsAPI.RevertEnvironmentVersion(context.Background(), environmentId, versionId).EnvironmentVersionRevertRequest(environmentVersionRevertRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EnvironmentsVersionsAPI.RevertEnvironmentVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RevertEnvironmentVersion`: EnvironmentVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `EnvironmentsVersionsAPI.RevertEnvironmentVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**environmentId** | **string** | A unique value identifying the environment. | 
**versionId** | **string** | A unique value identifying the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRevertEnvironmentVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **environmentVersionRevertRequest** | [**EnvironmentVersionRevertRequest**](EnvironmentVersionRevertRequest.md) |  | 

### Return type

[**EnvironmentVersionMeta**](EnvironmentVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

