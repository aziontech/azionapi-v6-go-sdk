# \ApplicationsDeviceGroupsAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateApplicationVersionDeviceGroups**](ApplicationsDeviceGroupsAPI.md#CreateApplicationVersionDeviceGroups) | **Post** /workspace/applications/{application_id}/versions/{version_id}/device_groups | Create an Applications Device Group
[**CreateDeviceGroup**](ApplicationsDeviceGroupsAPI.md#CreateDeviceGroup) | **Post** /workspace/applications/{application_id}/device_groups | Create an Applications Device Group
[**DeleteApplicationVersionDeviceGroup**](ApplicationsDeviceGroupsAPI.md#DeleteApplicationVersionDeviceGroup) | **Delete** /workspace/applications/{application_id}/versions/{version_id}/device_groups/{device_group_id} | Delete an Applications Device Group
[**DeleteDeviceGroup**](ApplicationsDeviceGroupsAPI.md#DeleteDeviceGroup) | **Delete** /workspace/applications/{application_id}/device_groups/{device_group_id} | Delete an Applications Device Group
[**ListApplicationVersionDeviceGroups**](ApplicationsDeviceGroupsAPI.md#ListApplicationVersionDeviceGroups) | **Get** /workspace/applications/{application_id}/versions/{version_id}/device_groups | List Applications Device Groups
[**ListDeviceGroups**](ApplicationsDeviceGroupsAPI.md#ListDeviceGroups) | **Get** /workspace/applications/{application_id}/device_groups | List Applications Device Groups
[**PartialUpdateApplicationVersionDeviceGroup**](ApplicationsDeviceGroupsAPI.md#PartialUpdateApplicationVersionDeviceGroup) | **Patch** /workspace/applications/{application_id}/versions/{version_id}/device_groups/{device_group_id} | Partially update an Applications Device Group
[**PartialUpdateDeviceGroup**](ApplicationsDeviceGroupsAPI.md#PartialUpdateDeviceGroup) | **Patch** /workspace/applications/{application_id}/device_groups/{device_group_id} | Partially update an Applications Device Group
[**RetrieveApplicationVersionDeviceGroup**](ApplicationsDeviceGroupsAPI.md#RetrieveApplicationVersionDeviceGroup) | **Get** /workspace/applications/{application_id}/versions/{version_id}/device_groups/{device_group_id} | Retrieve details of a Device Group
[**RetrieveDeviceGroup**](ApplicationsDeviceGroupsAPI.md#RetrieveDeviceGroup) | **Get** /workspace/applications/{application_id}/device_groups/{device_group_id} | Retrieve details of a Device Group
[**UpdateApplicationVersionDeviceGroup**](ApplicationsDeviceGroupsAPI.md#UpdateApplicationVersionDeviceGroup) | **Put** /workspace/applications/{application_id}/versions/{version_id}/device_groups/{device_group_id} | Update an Applications Device Group
[**UpdateDeviceGroup**](ApplicationsDeviceGroupsAPI.md#UpdateDeviceGroup) | **Put** /workspace/applications/{application_id}/device_groups/{device_group_id} | Update an Applications Device Group



## CreateApplicationVersionDeviceGroups

> DeviceGroupResponse CreateApplicationVersionDeviceGroups(ctx, applicationId, versionId).DeviceGroupRequest(deviceGroupRequest).Execute()

Create an Applications Device Group



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
	applicationId := int64(789) // int64 | A unique integer value identifying the application.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	deviceGroupRequest := *openapiclient.NewDeviceGroupRequest("Name_example", "UserAgent_example") // DeviceGroupRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsDeviceGroupsAPI.CreateApplicationVersionDeviceGroups(context.Background(), applicationId, versionId).DeviceGroupRequest(deviceGroupRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsDeviceGroupsAPI.CreateApplicationVersionDeviceGroups``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateApplicationVersionDeviceGroups`: DeviceGroupResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsDeviceGroupsAPI.CreateApplicationVersionDeviceGroups`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateApplicationVersionDeviceGroupsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **deviceGroupRequest** | [**DeviceGroupRequest**](DeviceGroupRequest.md) |  | 

### Return type

[**DeviceGroupResponse**](DeviceGroupResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateDeviceGroup

> DeviceGroupResponse CreateDeviceGroup(ctx, applicationId).DeviceGroupRequest(deviceGroupRequest).Execute()

Create an Applications Device Group



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
	applicationId := int64(789) // int64 | A unique integer value identifying the application.
	deviceGroupRequest := *openapiclient.NewDeviceGroupRequest("Name_example", "UserAgent_example") // DeviceGroupRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsDeviceGroupsAPI.CreateDeviceGroup(context.Background(), applicationId).DeviceGroupRequest(deviceGroupRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsDeviceGroupsAPI.CreateDeviceGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateDeviceGroup`: DeviceGroupResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsDeviceGroupsAPI.CreateDeviceGroup`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateDeviceGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **deviceGroupRequest** | [**DeviceGroupRequest**](DeviceGroupRequest.md) |  | 

### Return type

[**DeviceGroupResponse**](DeviceGroupResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteApplicationVersionDeviceGroup

> DeleteResponse DeleteApplicationVersionDeviceGroup(ctx, applicationId, deviceGroupId, versionId).Execute()

Delete an Applications Device Group



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
	applicationId := int64(789) // int64 | A unique integer value identifying the application.
	deviceGroupId := int64(789) // int64 | A unique integer value identifying the device group.
	versionId := "versionId_example" // string | The ULID identifier of the version.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsDeviceGroupsAPI.DeleteApplicationVersionDeviceGroup(context.Background(), applicationId, deviceGroupId, versionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsDeviceGroupsAPI.DeleteApplicationVersionDeviceGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteApplicationVersionDeviceGroup`: DeleteResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsDeviceGroupsAPI.DeleteApplicationVersionDeviceGroup`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**deviceGroupId** | **int64** | A unique integer value identifying the device group. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteApplicationVersionDeviceGroupRequest struct via the builder pattern


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


## DeleteDeviceGroup

> DeleteResponse DeleteDeviceGroup(ctx, applicationId, deviceGroupId).Execute()

Delete an Applications Device Group



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
	applicationId := int64(789) // int64 | A unique integer value identifying the application.
	deviceGroupId := int64(789) // int64 | A unique integer value identifying the device group.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsDeviceGroupsAPI.DeleteDeviceGroup(context.Background(), applicationId, deviceGroupId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsDeviceGroupsAPI.DeleteDeviceGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteDeviceGroup`: DeleteResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsDeviceGroupsAPI.DeleteDeviceGroup`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**deviceGroupId** | **int64** | A unique integer value identifying the device group. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDeviceGroupRequest struct via the builder pattern


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


## ListApplicationVersionDeviceGroups

> PaginatedDeviceGroupList ListApplicationVersionDeviceGroups(ctx, applicationId, versionId).Fields(fields).Id(id).Name(name).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).UserAgent(userAgent).Execute()

List Applications Device Groups



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
	applicationId := int64(789) // int64 | A unique integer value identifying the application.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	id := int64(789) // int64 | Filter by id (accepts comma-separated values). (optional)
	name := "name_example" // string | Filter by name (case-insensitive, partial match). (optional)
	ordering := "ordering_example" // string | Which field to use when ordering the results. (Valid fields: id, name, user_agent) (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	search := "search_example" // string | A search term to filter results. Searches across the following fields: name, user_agent. (optional)
	userAgent := "userAgent_example" // string | Filter by user agent (case-insensitive, partial match). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsDeviceGroupsAPI.ListApplicationVersionDeviceGroups(context.Background(), applicationId, versionId).Fields(fields).Id(id).Name(name).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).UserAgent(userAgent).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsDeviceGroupsAPI.ListApplicationVersionDeviceGroups``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListApplicationVersionDeviceGroups`: PaginatedDeviceGroupList
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsDeviceGroupsAPI.ListApplicationVersionDeviceGroups`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListApplicationVersionDeviceGroupsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **id** | **int64** | Filter by id (accepts comma-separated values). | 
 **name** | **string** | Filter by name (case-insensitive, partial match). | 
 **ordering** | **string** | Which field to use when ordering the results. (Valid fields: id, name, user_agent) | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **search** | **string** | A search term to filter results. Searches across the following fields: name, user_agent. | 
 **userAgent** | **string** | Filter by user agent (case-insensitive, partial match). | 

### Return type

[**PaginatedDeviceGroupList**](PaginatedDeviceGroupList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDeviceGroups

> PaginatedDeviceGroupList ListDeviceGroups(ctx, applicationId).Fields(fields).Id(id).Name(name).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).UserAgent(userAgent).Execute()

List Applications Device Groups



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
	applicationId := int64(789) // int64 | A unique integer value identifying the application.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	id := int64(789) // int64 | Filter by id (accepts comma-separated values). (optional)
	name := "name_example" // string | Filter by name (case-insensitive, partial match). (optional)
	ordering := "ordering_example" // string | Which field to use when ordering the results. (Valid fields: id, name, user_agent) (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	search := "search_example" // string | A search term to filter results. Searches across the following fields: name, user_agent. (optional)
	userAgent := "userAgent_example" // string | Filter by user agent (case-insensitive, partial match). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsDeviceGroupsAPI.ListDeviceGroups(context.Background(), applicationId).Fields(fields).Id(id).Name(name).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).UserAgent(userAgent).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsDeviceGroupsAPI.ListDeviceGroups``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDeviceGroups`: PaginatedDeviceGroupList
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsDeviceGroupsAPI.ListDeviceGroups`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListDeviceGroupsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **id** | **int64** | Filter by id (accepts comma-separated values). | 
 **name** | **string** | Filter by name (case-insensitive, partial match). | 
 **ordering** | **string** | Which field to use when ordering the results. (Valid fields: id, name, user_agent) | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **search** | **string** | A search term to filter results. Searches across the following fields: name, user_agent. | 
 **userAgent** | **string** | Filter by user agent (case-insensitive, partial match). | 

### Return type

[**PaginatedDeviceGroupList**](PaginatedDeviceGroupList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateApplicationVersionDeviceGroup

> DeviceGroupResponse PartialUpdateApplicationVersionDeviceGroup(ctx, applicationId, deviceGroupId, versionId).PatchedDeviceGroupRequest(patchedDeviceGroupRequest).Execute()

Partially update an Applications Device Group



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
	applicationId := int64(789) // int64 | A unique integer value identifying the application.
	deviceGroupId := int64(789) // int64 | A unique integer value identifying the device group.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	patchedDeviceGroupRequest := *openapiclient.NewPatchedDeviceGroupRequest() // PatchedDeviceGroupRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsDeviceGroupsAPI.PartialUpdateApplicationVersionDeviceGroup(context.Background(), applicationId, deviceGroupId, versionId).PatchedDeviceGroupRequest(patchedDeviceGroupRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsDeviceGroupsAPI.PartialUpdateApplicationVersionDeviceGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateApplicationVersionDeviceGroup`: DeviceGroupResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsDeviceGroupsAPI.PartialUpdateApplicationVersionDeviceGroup`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**deviceGroupId** | **int64** | A unique integer value identifying the device group. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateApplicationVersionDeviceGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **patchedDeviceGroupRequest** | [**PatchedDeviceGroupRequest**](PatchedDeviceGroupRequest.md) |  | 

### Return type

[**DeviceGroupResponse**](DeviceGroupResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateDeviceGroup

> DeviceGroupResponse PartialUpdateDeviceGroup(ctx, applicationId, deviceGroupId).PatchedDeviceGroupRequest(patchedDeviceGroupRequest).Execute()

Partially update an Applications Device Group



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
	applicationId := int64(789) // int64 | A unique integer value identifying the application.
	deviceGroupId := int64(789) // int64 | A unique integer value identifying the device group.
	patchedDeviceGroupRequest := *openapiclient.NewPatchedDeviceGroupRequest() // PatchedDeviceGroupRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsDeviceGroupsAPI.PartialUpdateDeviceGroup(context.Background(), applicationId, deviceGroupId).PatchedDeviceGroupRequest(patchedDeviceGroupRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsDeviceGroupsAPI.PartialUpdateDeviceGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateDeviceGroup`: DeviceGroupResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsDeviceGroupsAPI.PartialUpdateDeviceGroup`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**deviceGroupId** | **int64** | A unique integer value identifying the device group. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateDeviceGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **patchedDeviceGroupRequest** | [**PatchedDeviceGroupRequest**](PatchedDeviceGroupRequest.md) |  | 

### Return type

[**DeviceGroupResponse**](DeviceGroupResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveApplicationVersionDeviceGroup

> DeviceGroupRetrieveResponse RetrieveApplicationVersionDeviceGroup(ctx, applicationId, deviceGroupId, versionId).Fields(fields).Execute()

Retrieve details of a Device Group



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
	applicationId := int64(789) // int64 | A unique integer value identifying the application.
	deviceGroupId := int64(789) // int64 | A unique integer value identifying the device group.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsDeviceGroupsAPI.RetrieveApplicationVersionDeviceGroup(context.Background(), applicationId, deviceGroupId, versionId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsDeviceGroupsAPI.RetrieveApplicationVersionDeviceGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveApplicationVersionDeviceGroup`: DeviceGroupRetrieveResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsDeviceGroupsAPI.RetrieveApplicationVersionDeviceGroup`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**deviceGroupId** | **int64** | A unique integer value identifying the device group. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveApplicationVersionDeviceGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**DeviceGroupRetrieveResponse**](DeviceGroupRetrieveResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveDeviceGroup

> DeviceGroupRetrieveResponse RetrieveDeviceGroup(ctx, applicationId, deviceGroupId).Fields(fields).Execute()

Retrieve details of a Device Group



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
	applicationId := int64(789) // int64 | A unique integer value identifying the application.
	deviceGroupId := int64(789) // int64 | A unique integer value identifying the device group.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsDeviceGroupsAPI.RetrieveDeviceGroup(context.Background(), applicationId, deviceGroupId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsDeviceGroupsAPI.RetrieveDeviceGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveDeviceGroup`: DeviceGroupRetrieveResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsDeviceGroupsAPI.RetrieveDeviceGroup`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**deviceGroupId** | **int64** | A unique integer value identifying the device group. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveDeviceGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**DeviceGroupRetrieveResponse**](DeviceGroupRetrieveResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateApplicationVersionDeviceGroup

> DeviceGroupResponse UpdateApplicationVersionDeviceGroup(ctx, applicationId, deviceGroupId, versionId).DeviceGroupRequest(deviceGroupRequest).Execute()

Update an Applications Device Group



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
	applicationId := int64(789) // int64 | A unique integer value identifying the application.
	deviceGroupId := int64(789) // int64 | A unique integer value identifying the device group.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	deviceGroupRequest := *openapiclient.NewDeviceGroupRequest("Name_example", "UserAgent_example") // DeviceGroupRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsDeviceGroupsAPI.UpdateApplicationVersionDeviceGroup(context.Background(), applicationId, deviceGroupId, versionId).DeviceGroupRequest(deviceGroupRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsDeviceGroupsAPI.UpdateApplicationVersionDeviceGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateApplicationVersionDeviceGroup`: DeviceGroupResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsDeviceGroupsAPI.UpdateApplicationVersionDeviceGroup`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**deviceGroupId** | **int64** | A unique integer value identifying the device group. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateApplicationVersionDeviceGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **deviceGroupRequest** | [**DeviceGroupRequest**](DeviceGroupRequest.md) |  | 

### Return type

[**DeviceGroupResponse**](DeviceGroupResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateDeviceGroup

> DeviceGroupResponse UpdateDeviceGroup(ctx, applicationId, deviceGroupId).DeviceGroupRequest(deviceGroupRequest).Execute()

Update an Applications Device Group



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
	applicationId := int64(789) // int64 | A unique integer value identifying the application.
	deviceGroupId := int64(789) // int64 | A unique integer value identifying the device group.
	deviceGroupRequest := *openapiclient.NewDeviceGroupRequest("Name_example", "UserAgent_example") // DeviceGroupRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsDeviceGroupsAPI.UpdateDeviceGroup(context.Background(), applicationId, deviceGroupId).DeviceGroupRequest(deviceGroupRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsDeviceGroupsAPI.UpdateDeviceGroup``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateDeviceGroup`: DeviceGroupResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsDeviceGroupsAPI.UpdateDeviceGroup`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**deviceGroupId** | **int64** | A unique integer value identifying the device group. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateDeviceGroupRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **deviceGroupRequest** | [**DeviceGroupRequest**](DeviceGroupRequest.md) |  | 

### Return type

[**DeviceGroupResponse**](DeviceGroupResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

