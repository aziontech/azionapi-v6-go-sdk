# \ApplicationsCacheSettingsAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateApplicationVersionCacheSettings**](ApplicationsCacheSettingsAPI.md#CreateApplicationVersionCacheSettings) | **Post** /workspace/applications/{application_id}/versions/{version_id}/cache_settings | Create an Applications Cache Setting
[**CreateCacheSetting**](ApplicationsCacheSettingsAPI.md#CreateCacheSetting) | **Post** /workspace/applications/{application_id}/cache_settings | Create an Applications Cache Setting
[**DeleteApplicationVersionCacheSetting**](ApplicationsCacheSettingsAPI.md#DeleteApplicationVersionCacheSetting) | **Delete** /workspace/applications/{application_id}/versions/{version_id}/cache_settings/{cache_setting_id} | Delete an Applications Cache Setting
[**DeleteCacheSetting**](ApplicationsCacheSettingsAPI.md#DeleteCacheSetting) | **Delete** /workspace/applications/{application_id}/cache_settings/{cache_setting_id} | Delete an Applications Cache Setting
[**ListApplicationVersionCacheSettings**](ApplicationsCacheSettingsAPI.md#ListApplicationVersionCacheSettings) | **Get** /workspace/applications/{application_id}/versions/{version_id}/cache_settings | List all Applications Cache Settings
[**ListCacheSettings**](ApplicationsCacheSettingsAPI.md#ListCacheSettings) | **Get** /workspace/applications/{application_id}/cache_settings | List all Applications Cache Settings
[**PartialUpdateApplicationVersionCacheSetting**](ApplicationsCacheSettingsAPI.md#PartialUpdateApplicationVersionCacheSetting) | **Patch** /workspace/applications/{application_id}/versions/{version_id}/cache_settings/{cache_setting_id} | Partially update an Applications Cache Setting
[**PartialUpdateCacheSetting**](ApplicationsCacheSettingsAPI.md#PartialUpdateCacheSetting) | **Patch** /workspace/applications/{application_id}/cache_settings/{cache_setting_id} | Partially update an Applications Cache Setting
[**RetrieveApplicationVersionCacheSetting**](ApplicationsCacheSettingsAPI.md#RetrieveApplicationVersionCacheSetting) | **Get** /workspace/applications/{application_id}/versions/{version_id}/cache_settings/{cache_setting_id} | Retrieve details of an Applications Cache Setting
[**RetrieveCacheSetting**](ApplicationsCacheSettingsAPI.md#RetrieveCacheSetting) | **Get** /workspace/applications/{application_id}/cache_settings/{cache_setting_id} | Retrieve details of an Applications Cache Setting
[**UpdateApplicationVersionCacheSetting**](ApplicationsCacheSettingsAPI.md#UpdateApplicationVersionCacheSetting) | **Put** /workspace/applications/{application_id}/versions/{version_id}/cache_settings/{cache_setting_id} | Update an Applications Cache Setting
[**UpdateCacheSetting**](ApplicationsCacheSettingsAPI.md#UpdateCacheSetting) | **Put** /workspace/applications/{application_id}/cache_settings/{cache_setting_id} | Update an Applications Cache Setting



## CreateApplicationVersionCacheSettings

> CacheSettingResponse CreateApplicationVersionCacheSettings(ctx, applicationId, versionId).CacheSettingRequest(cacheSettingRequest).Execute()

Create an Applications Cache Setting



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
	cacheSettingRequest := *openapiclient.NewCacheSettingRequest("Name_example") // CacheSettingRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsCacheSettingsAPI.CreateApplicationVersionCacheSettings(context.Background(), applicationId, versionId).CacheSettingRequest(cacheSettingRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsCacheSettingsAPI.CreateApplicationVersionCacheSettings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateApplicationVersionCacheSettings`: CacheSettingResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsCacheSettingsAPI.CreateApplicationVersionCacheSettings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateApplicationVersionCacheSettingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **cacheSettingRequest** | [**CacheSettingRequest**](CacheSettingRequest.md) |  | 

### Return type

[**CacheSettingResponse**](CacheSettingResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateCacheSetting

> CacheSettingResponse CreateCacheSetting(ctx, applicationId).CacheSettingRequest(cacheSettingRequest).Execute()

Create an Applications Cache Setting



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
	cacheSettingRequest := *openapiclient.NewCacheSettingRequest("Name_example") // CacheSettingRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsCacheSettingsAPI.CreateCacheSetting(context.Background(), applicationId).CacheSettingRequest(cacheSettingRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsCacheSettingsAPI.CreateCacheSetting``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateCacheSetting`: CacheSettingResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsCacheSettingsAPI.CreateCacheSetting`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateCacheSettingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **cacheSettingRequest** | [**CacheSettingRequest**](CacheSettingRequest.md) |  | 

### Return type

[**CacheSettingResponse**](CacheSettingResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteApplicationVersionCacheSetting

> DeleteResponse DeleteApplicationVersionCacheSetting(ctx, applicationId, cacheSettingId, versionId).Execute()

Delete an Applications Cache Setting



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
	cacheSettingId := int64(789) // int64 | A unique integer value identifying the cache setting.
	versionId := "versionId_example" // string | The ULID identifier of the version.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsCacheSettingsAPI.DeleteApplicationVersionCacheSetting(context.Background(), applicationId, cacheSettingId, versionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsCacheSettingsAPI.DeleteApplicationVersionCacheSetting``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteApplicationVersionCacheSetting`: DeleteResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsCacheSettingsAPI.DeleteApplicationVersionCacheSetting`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**cacheSettingId** | **int64** | A unique integer value identifying the cache setting. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteApplicationVersionCacheSettingRequest struct via the builder pattern


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


## DeleteCacheSetting

> DeleteResponse DeleteCacheSetting(ctx, applicationId, cacheSettingId).Execute()

Delete an Applications Cache Setting



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
	cacheSettingId := int64(789) // int64 | A unique integer value identifying the cache setting.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsCacheSettingsAPI.DeleteCacheSetting(context.Background(), applicationId, cacheSettingId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsCacheSettingsAPI.DeleteCacheSetting``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteCacheSetting`: DeleteResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsCacheSettingsAPI.DeleteCacheSetting`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**cacheSettingId** | **int64** | A unique integer value identifying the cache setting. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteCacheSettingRequest struct via the builder pattern


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


## ListApplicationVersionCacheSettings

> PaginatedCacheSettingList ListApplicationVersionCacheSettings(ctx, applicationId, versionId).Fields(fields).Id(id).Name(name).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()

List all Applications Cache Settings



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
	ordering := "ordering_example" // string | Which field to use when ordering the results. (Valid fields: id, name, browser_cache_settings, cdn_cache_settings, cache_by_query_string, cache_by_cookies, adaptive_delivery_action, enable_caching_for_post, enable_caching_for_options, enable_stale_cache, l2_caching_enabled) (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	search := "search_example" // string | A search term to filter results. Searches across the following fields: name, cdn_cache_settings, cache_by_query_string, query_string_fields, cache_by_cookies, cookie_names, adaptive_delivery_action. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsCacheSettingsAPI.ListApplicationVersionCacheSettings(context.Background(), applicationId, versionId).Fields(fields).Id(id).Name(name).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsCacheSettingsAPI.ListApplicationVersionCacheSettings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListApplicationVersionCacheSettings`: PaginatedCacheSettingList
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsCacheSettingsAPI.ListApplicationVersionCacheSettings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListApplicationVersionCacheSettingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **id** | **int64** | Filter by id (accepts comma-separated values). | 
 **name** | **string** | Filter by name (case-insensitive, partial match). | 
 **ordering** | **string** | Which field to use when ordering the results. (Valid fields: id, name, browser_cache_settings, cdn_cache_settings, cache_by_query_string, cache_by_cookies, adaptive_delivery_action, enable_caching_for_post, enable_caching_for_options, enable_stale_cache, l2_caching_enabled) | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **search** | **string** | A search term to filter results. Searches across the following fields: name, cdn_cache_settings, cache_by_query_string, query_string_fields, cache_by_cookies, cookie_names, adaptive_delivery_action. | 

### Return type

[**PaginatedCacheSettingList**](PaginatedCacheSettingList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCacheSettings

> PaginatedCacheSettingList ListCacheSettings(ctx, applicationId).Fields(fields).Id(id).Name(name).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()

List all Applications Cache Settings



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
	ordering := "ordering_example" // string | Which field to use when ordering the results. (Valid fields: id, name, browser_cache_settings, cdn_cache_settings, cache_by_query_string, cache_by_cookies, adaptive_delivery_action, enable_caching_for_post, enable_caching_for_options, enable_stale_cache, l2_caching_enabled) (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	search := "search_example" // string | A search term to filter results. Searches across the following fields: name, cdn_cache_settings, cache_by_query_string, query_string_fields, cache_by_cookies, cookie_names, adaptive_delivery_action. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsCacheSettingsAPI.ListCacheSettings(context.Background(), applicationId).Fields(fields).Id(id).Name(name).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsCacheSettingsAPI.ListCacheSettings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCacheSettings`: PaginatedCacheSettingList
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsCacheSettingsAPI.ListCacheSettings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListCacheSettingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **id** | **int64** | Filter by id (accepts comma-separated values). | 
 **name** | **string** | Filter by name (case-insensitive, partial match). | 
 **ordering** | **string** | Which field to use when ordering the results. (Valid fields: id, name, browser_cache_settings, cdn_cache_settings, cache_by_query_string, cache_by_cookies, adaptive_delivery_action, enable_caching_for_post, enable_caching_for_options, enable_stale_cache, l2_caching_enabled) | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **search** | **string** | A search term to filter results. Searches across the following fields: name, cdn_cache_settings, cache_by_query_string, query_string_fields, cache_by_cookies, cookie_names, adaptive_delivery_action. | 

### Return type

[**PaginatedCacheSettingList**](PaginatedCacheSettingList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateApplicationVersionCacheSetting

> CacheSettingResponse PartialUpdateApplicationVersionCacheSetting(ctx, applicationId, cacheSettingId, versionId).PatchedCacheSettingRequest(patchedCacheSettingRequest).Execute()

Partially update an Applications Cache Setting



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
	cacheSettingId := int64(789) // int64 | A unique integer value identifying the cache setting.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	patchedCacheSettingRequest := *openapiclient.NewPatchedCacheSettingRequest() // PatchedCacheSettingRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsCacheSettingsAPI.PartialUpdateApplicationVersionCacheSetting(context.Background(), applicationId, cacheSettingId, versionId).PatchedCacheSettingRequest(patchedCacheSettingRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsCacheSettingsAPI.PartialUpdateApplicationVersionCacheSetting``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateApplicationVersionCacheSetting`: CacheSettingResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsCacheSettingsAPI.PartialUpdateApplicationVersionCacheSetting`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**cacheSettingId** | **int64** | A unique integer value identifying the cache setting. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateApplicationVersionCacheSettingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **patchedCacheSettingRequest** | [**PatchedCacheSettingRequest**](PatchedCacheSettingRequest.md) |  | 

### Return type

[**CacheSettingResponse**](CacheSettingResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateCacheSetting

> CacheSettingResponse PartialUpdateCacheSetting(ctx, applicationId, cacheSettingId).PatchedCacheSettingRequest(patchedCacheSettingRequest).Execute()

Partially update an Applications Cache Setting



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
	cacheSettingId := int64(789) // int64 | A unique integer value identifying the cache setting.
	patchedCacheSettingRequest := *openapiclient.NewPatchedCacheSettingRequest() // PatchedCacheSettingRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsCacheSettingsAPI.PartialUpdateCacheSetting(context.Background(), applicationId, cacheSettingId).PatchedCacheSettingRequest(patchedCacheSettingRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsCacheSettingsAPI.PartialUpdateCacheSetting``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateCacheSetting`: CacheSettingResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsCacheSettingsAPI.PartialUpdateCacheSetting`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**cacheSettingId** | **int64** | A unique integer value identifying the cache setting. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateCacheSettingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **patchedCacheSettingRequest** | [**PatchedCacheSettingRequest**](PatchedCacheSettingRequest.md) |  | 

### Return type

[**CacheSettingResponse**](CacheSettingResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveApplicationVersionCacheSetting

> CacheSettingRetrieveResponse RetrieveApplicationVersionCacheSetting(ctx, applicationId, cacheSettingId, versionId).Fields(fields).Execute()

Retrieve details of an Applications Cache Setting



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
	cacheSettingId := int64(789) // int64 | A unique integer value identifying the cache setting.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsCacheSettingsAPI.RetrieveApplicationVersionCacheSetting(context.Background(), applicationId, cacheSettingId, versionId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsCacheSettingsAPI.RetrieveApplicationVersionCacheSetting``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveApplicationVersionCacheSetting`: CacheSettingRetrieveResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsCacheSettingsAPI.RetrieveApplicationVersionCacheSetting`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**cacheSettingId** | **int64** | A unique integer value identifying the cache setting. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveApplicationVersionCacheSettingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**CacheSettingRetrieveResponse**](CacheSettingRetrieveResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveCacheSetting

> CacheSettingRetrieveResponse RetrieveCacheSetting(ctx, applicationId, cacheSettingId).Fields(fields).Execute()

Retrieve details of an Applications Cache Setting



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
	cacheSettingId := int64(789) // int64 | A unique integer value identifying the cache setting.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsCacheSettingsAPI.RetrieveCacheSetting(context.Background(), applicationId, cacheSettingId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsCacheSettingsAPI.RetrieveCacheSetting``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveCacheSetting`: CacheSettingRetrieveResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsCacheSettingsAPI.RetrieveCacheSetting`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**cacheSettingId** | **int64** | A unique integer value identifying the cache setting. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveCacheSettingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**CacheSettingRetrieveResponse**](CacheSettingRetrieveResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateApplicationVersionCacheSetting

> CacheSettingResponse UpdateApplicationVersionCacheSetting(ctx, applicationId, cacheSettingId, versionId).CacheSettingRequest(cacheSettingRequest).Execute()

Update an Applications Cache Setting



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
	cacheSettingId := int64(789) // int64 | A unique integer value identifying the cache setting.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	cacheSettingRequest := *openapiclient.NewCacheSettingRequest("Name_example") // CacheSettingRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsCacheSettingsAPI.UpdateApplicationVersionCacheSetting(context.Background(), applicationId, cacheSettingId, versionId).CacheSettingRequest(cacheSettingRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsCacheSettingsAPI.UpdateApplicationVersionCacheSetting``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateApplicationVersionCacheSetting`: CacheSettingResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsCacheSettingsAPI.UpdateApplicationVersionCacheSetting`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**cacheSettingId** | **int64** | A unique integer value identifying the cache setting. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateApplicationVersionCacheSettingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **cacheSettingRequest** | [**CacheSettingRequest**](CacheSettingRequest.md) |  | 

### Return type

[**CacheSettingResponse**](CacheSettingResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateCacheSetting

> CacheSettingResponse UpdateCacheSetting(ctx, applicationId, cacheSettingId).CacheSettingRequest(cacheSettingRequest).Execute()

Update an Applications Cache Setting



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
	cacheSettingId := int64(789) // int64 | A unique integer value identifying the cache setting.
	cacheSettingRequest := *openapiclient.NewCacheSettingRequest("Name_example") // CacheSettingRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsCacheSettingsAPI.UpdateCacheSetting(context.Background(), applicationId, cacheSettingId).CacheSettingRequest(cacheSettingRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsCacheSettingsAPI.UpdateCacheSetting``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateCacheSetting`: CacheSettingResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsCacheSettingsAPI.UpdateCacheSetting`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**cacheSettingId** | **int64** | A unique integer value identifying the cache setting. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateCacheSettingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **cacheSettingRequest** | [**CacheSettingRequest**](CacheSettingRequest.md) |  | 

### Return type

[**CacheSettingResponse**](CacheSettingResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

