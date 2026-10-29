# \DeploymentsResourceUsageAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListResourceUsage**](DeploymentsResourceUsageAPI.md#ListResourceUsage) | **Get** /resource_usage | List deployments using a resource
[**RetrieveDeploymentResourceHierarchy**](DeploymentsResourceUsageAPI.md#RetrieveDeploymentResourceHierarchy) | **Get** /deployments/{deployment_id}/resource_hierarchy | Get a deployment resource hierarchy



## ListResourceUsage

> PaginatedResourceUsageList ListResourceUsage(ctx).ResourceId(resourceId).ResourceType(resourceType).Fields(fields).Page(page).PageSize(pageSize).Execute()

List deployments using a resource



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
	resourceId := []string{"Inner_example"} // []string | One or more resource ids to look up (for `application` this is its `global_id`). Repeat the key (`resource_id=a&resource_id=b`) or pass a comma-separated list (`resource_id=a,b`). Max 100.
	resourceType := "resourceType_example" // string | Resource type to look up.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsResourceUsageAPI.ListResourceUsage(context.Background()).ResourceId(resourceId).ResourceType(resourceType).Fields(fields).Page(page).PageSize(pageSize).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsResourceUsageAPI.ListResourceUsage``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListResourceUsage`: PaginatedResourceUsageList
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsResourceUsageAPI.ListResourceUsage`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListResourceUsageRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **resourceId** | **[]string** | One or more resource ids to look up (for &#x60;application&#x60; this is its &#x60;global_id&#x60;). Repeat the key (&#x60;resource_id&#x3D;a&amp;resource_id&#x3D;b&#x60;) or pass a comma-separated list (&#x60;resource_id&#x3D;a,b&#x60;). Max 100. | 
 **resourceType** | **string** | Resource type to look up. | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 

### Return type

[**PaginatedResourceUsageList**](PaginatedResourceUsageList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveDeploymentResourceHierarchy

> ResourceHierarchyResponse RetrieveDeploymentResourceHierarchy(ctx, deploymentId).Fields(fields).Execute()

Get a deployment resource hierarchy



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
	deploymentId := "deploymentId_example" // string | A unique value identifying the deployment.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsResourceUsageAPI.RetrieveDeploymentResourceHierarchy(context.Background(), deploymentId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsResourceUsageAPI.RetrieveDeploymentResourceHierarchy``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveDeploymentResourceHierarchy`: ResourceHierarchyResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsResourceUsageAPI.RetrieveDeploymentResourceHierarchy`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveDeploymentResourceHierarchyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**ResourceHierarchyResponse**](ResourceHierarchyResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

