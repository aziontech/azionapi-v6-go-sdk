# \DeploymentsAPI

All URIs are relative to *https://stage-api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateDeployment**](DeploymentsAPI.md#CreateDeployment) | **Post** /deployments | Create a Deployment
[**DeleteDeployment**](DeploymentsAPI.md#DeleteDeployment) | **Delete** /deployments/{deployment_id} | Delete a Deployment
[**ListDeployments**](DeploymentsAPI.md#ListDeployments) | **Get** /deployments | List Deployments
[**PartialUpdateDeployment**](DeploymentsAPI.md#PartialUpdateDeployment) | **Patch** /deployments/{deployment_id} | Partially update a Deployment
[**RetrieveDeployment**](DeploymentsAPI.md#RetrieveDeployment) | **Get** /deployments/{deployment_id} | Retrieve details of a Deployment
[**UpdateDeployment**](DeploymentsAPI.md#UpdateDeployment) | **Put** /deployments/{deployment_id} | Update a Deployment



## CreateDeployment

> DeploymentResponse CreateDeployment(ctx).DeploymentCreateRequest(deploymentCreateRequest).Execute()

Create a Deployment



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
	deploymentCreateRequest := *openapiclient.NewDeploymentCreateRequest("Name_example", "BindingPolicy_example") // DeploymentCreateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsAPI.CreateDeployment(context.Background()).DeploymentCreateRequest(deploymentCreateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsAPI.CreateDeployment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateDeployment`: DeploymentResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsAPI.CreateDeployment`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateDeploymentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deploymentCreateRequest** | [**DeploymentCreateRequest**](DeploymentCreateRequest.md) |  | 

### Return type

[**DeploymentResponse**](DeploymentResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteDeployment

> DeleteDeployment(ctx, deploymentId).Execute()

Delete a Deployment



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.DeploymentsAPI.DeleteDeployment(context.Background(), deploymentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsAPI.DeleteDeployment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDeploymentRequest struct via the builder pattern


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


## ListDeployments

> PaginatedDeploymentList ListDeployments(ctx).BindingPolicy(bindingPolicy).CreatedAtGte(createdAtGte).CreatedAtLte(createdAtLte).DeploymentPolicy(deploymentPolicy).Fields(fields).Id(id).IdIn(idIn).LastModifiedGte(lastModifiedGte).LastModifiedLte(lastModifiedLte).Name(name).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).State(state).Execute()

List Deployments



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
	bindingPolicy := "bindingPolicy_example" // string | Filter by binding policy. (optional)
	createdAtGte := time.Now() // time.Time | Filter by creation date (greater than or equal). (optional)
	createdAtLte := time.Now() // time.Time | Filter by creation date (less than or equal). (optional)
	deploymentPolicy := "deploymentPolicy_example" // string | Filter by deployment policy. (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	id := []string{"Inner_example"} // []string | Filter by id (accepts comma-separated values). (optional)
	idIn := []string{"Inner_example"} // []string | Filter by id (accepts comma-separated values). (optional)
	lastModifiedGte := time.Now() // time.Time | Filter by last modified date (greater than or equal). (optional)
	lastModifiedLte := time.Now() // time.Time | Filter by last modified date (less than or equal). (optional)
	name := "name_example" // string | Filter by name (case-insensitive, partial match). (optional)
	ordering := "ordering_example" // string | Which field to use when ordering the results. (Valid fields: id, name, created_at, last_modified, version_state) (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	search := "search_example" // string | A search term to filter results. Searches across the following fields: name. (optional)
	state := []string{"Inner_example"} // []string | Filter by state (accepts comma-separated values). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsAPI.ListDeployments(context.Background()).BindingPolicy(bindingPolicy).CreatedAtGte(createdAtGte).CreatedAtLte(createdAtLte).DeploymentPolicy(deploymentPolicy).Fields(fields).Id(id).IdIn(idIn).LastModifiedGte(lastModifiedGte).LastModifiedLte(lastModifiedLte).Name(name).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).State(state).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsAPI.ListDeployments``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDeployments`: PaginatedDeploymentList
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsAPI.ListDeployments`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListDeploymentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bindingPolicy** | **string** | Filter by binding policy. | 
 **createdAtGte** | **time.Time** | Filter by creation date (greater than or equal). | 
 **createdAtLte** | **time.Time** | Filter by creation date (less than or equal). | 
 **deploymentPolicy** | **string** | Filter by deployment policy. | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **id** | **[]string** | Filter by id (accepts comma-separated values). | 
 **idIn** | **[]string** | Filter by id (accepts comma-separated values). | 
 **lastModifiedGte** | **time.Time** | Filter by last modified date (greater than or equal). | 
 **lastModifiedLte** | **time.Time** | Filter by last modified date (less than or equal). | 
 **name** | **string** | Filter by name (case-insensitive, partial match). | 
 **ordering** | **string** | Which field to use when ordering the results. (Valid fields: id, name, created_at, last_modified, version_state) | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **search** | **string** | A search term to filter results. Searches across the following fields: name. | 
 **state** | **[]string** | Filter by state (accepts comma-separated values). | 

### Return type

[**PaginatedDeploymentList**](PaginatedDeploymentList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateDeployment

> DeploymentResponse PartialUpdateDeployment(ctx, deploymentId).PatchedDeploymentRequest(patchedDeploymentRequest).Execute()

Partially update a Deployment



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
	patchedDeploymentRequest := *openapiclient.NewPatchedDeploymentRequest() // PatchedDeploymentRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsAPI.PartialUpdateDeployment(context.Background(), deploymentId).PatchedDeploymentRequest(patchedDeploymentRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsAPI.PartialUpdateDeployment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateDeployment`: DeploymentResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsAPI.PartialUpdateDeployment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateDeploymentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **patchedDeploymentRequest** | [**PatchedDeploymentRequest**](PatchedDeploymentRequest.md) |  | 

### Return type

[**DeploymentResponse**](DeploymentResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveDeployment

> DeploymentRetrieveResponse RetrieveDeployment(ctx, deploymentId).Fields(fields).Execute()

Retrieve details of a Deployment



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
	resp, r, err := apiClient.DeploymentsAPI.RetrieveDeployment(context.Background(), deploymentId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsAPI.RetrieveDeployment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveDeployment`: DeploymentRetrieveResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsAPI.RetrieveDeployment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveDeploymentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**DeploymentRetrieveResponse**](DeploymentRetrieveResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateDeployment

> DeploymentResponse UpdateDeployment(ctx, deploymentId).DeploymentRequest(deploymentRequest).Execute()

Update a Deployment



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
	deploymentRequest := *openapiclient.NewDeploymentRequest("Name_example", "Description_example", "BindingPolicy_example", *openapiclient.NewDeploymentStrategyDefaults()) // DeploymentRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsAPI.UpdateDeployment(context.Background(), deploymentId).DeploymentRequest(deploymentRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsAPI.UpdateDeployment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateDeployment`: DeploymentResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsAPI.UpdateDeployment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateDeploymentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **deploymentRequest** | [**DeploymentRequest**](DeploymentRequest.md) |  | 

### Return type

[**DeploymentResponse**](DeploymentResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

