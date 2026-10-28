# \ApplicationsRequestRulesAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateApplicationRequestRule**](ApplicationsRequestRulesAPI.md#CreateApplicationRequestRule) | **Post** /workspace/applications/{application_id}/request_rules | Create an Application Request Rule
[**CreateApplicationVersionRequestRules**](ApplicationsRequestRulesAPI.md#CreateApplicationVersionRequestRules) | **Post** /workspace/applications/{application_id}/versions/{version_id}/request_rules | Create an Application Request Rule
[**DeleteApplicationRequestRule**](ApplicationsRequestRulesAPI.md#DeleteApplicationRequestRule) | **Delete** /workspace/applications/{application_id}/request_rules/{request_rule_id} | Delete an Application Request Rule
[**DeleteApplicationVersionRequestRule**](ApplicationsRequestRulesAPI.md#DeleteApplicationVersionRequestRule) | **Delete** /workspace/applications/{application_id}/versions/{version_id}/request_rules/{request_rule_id} | Delete an Application Request Rule
[**ListApplicationRequestRules**](ApplicationsRequestRulesAPI.md#ListApplicationRequestRules) | **Get** /workspace/applications/{application_id}/request_rules | List Application Request Rules
[**ListApplicationVersionRequestRules**](ApplicationsRequestRulesAPI.md#ListApplicationVersionRequestRules) | **Get** /workspace/applications/{application_id}/versions/{version_id}/request_rules | List Application Request Rules
[**PartialUpdateApplicationRequestRule**](ApplicationsRequestRulesAPI.md#PartialUpdateApplicationRequestRule) | **Patch** /workspace/applications/{application_id}/request_rules/{request_rule_id} | Partially update an Application Request Rule
[**PartialUpdateApplicationVersionRequestRule**](ApplicationsRequestRulesAPI.md#PartialUpdateApplicationVersionRequestRule) | **Patch** /workspace/applications/{application_id}/versions/{version_id}/request_rules/{request_rule_id} | Partially update an Application Request Rule
[**RetrieveApplicationRequestRule**](ApplicationsRequestRulesAPI.md#RetrieveApplicationRequestRule) | **Get** /workspace/applications/{application_id}/request_rules/{request_rule_id} | Retrieve details of an Application Request Rule
[**RetrieveApplicationVersionRequestRule**](ApplicationsRequestRulesAPI.md#RetrieveApplicationVersionRequestRule) | **Get** /workspace/applications/{application_id}/versions/{version_id}/request_rules/{request_rule_id} | Retrieve details of an Application Request Rule
[**UpdateApplicationRequestRule**](ApplicationsRequestRulesAPI.md#UpdateApplicationRequestRule) | **Put** /workspace/applications/{application_id}/request_rules/{request_rule_id} | Update an Application Request Rule
[**UpdateApplicationRequestRulesOrder**](ApplicationsRequestRulesAPI.md#UpdateApplicationRequestRulesOrder) | **Put** /workspace/applications/{application_id}/request_rules/order | Ordering Application Request Rules
[**UpdateApplicationVersionRequestRule**](ApplicationsRequestRulesAPI.md#UpdateApplicationVersionRequestRule) | **Put** /workspace/applications/{application_id}/versions/{version_id}/request_rules/{request_rule_id} | Update an Application Request Rule
[**UpdateApplicationVersionRequestRulesOrder**](ApplicationsRequestRulesAPI.md#UpdateApplicationVersionRequestRulesOrder) | **Put** /workspace/applications/{application_id}/versions/{version_id}/request_rules/order | Ordering Application Request Rules



## CreateApplicationRequestRule

> RequestPhaseRuleResponse CreateApplicationRequestRule(ctx, applicationId).RequestPhaseRuleRequest(requestPhaseRuleRequest).Execute()

Create an Application Request Rule



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
	requestPhaseRuleRequest := *openapiclient.NewRequestPhaseRuleRequest("Name_example", [][]ApplicationCriterionFieldRequest{[]openapiclient.ApplicationCriterionFieldRequest{*openapiclient.NewApplicationCriterionFieldRequest("Conditional_example", "Variable_example", "Operator_example")}}, []openapiclient.RequestPhaseBehaviorRequest{openapiclient.RequestPhaseBehaviorRequest{BehaviorArgs: openapiclient.NewBehaviorArgs("Type_example", *openapiclient.NewBehaviorArgsAttributes(*openapiclient.NewBehaviorArgsAttributesValue()))}}) // RequestPhaseRuleRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsRequestRulesAPI.CreateApplicationRequestRule(context.Background(), applicationId).RequestPhaseRuleRequest(requestPhaseRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsRequestRulesAPI.CreateApplicationRequestRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateApplicationRequestRule`: RequestPhaseRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsRequestRulesAPI.CreateApplicationRequestRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateApplicationRequestRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **requestPhaseRuleRequest** | [**RequestPhaseRuleRequest**](RequestPhaseRuleRequest.md) |  | 

### Return type

[**RequestPhaseRuleResponse**](RequestPhaseRuleResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateApplicationVersionRequestRules

> RequestPhaseRuleResponse CreateApplicationVersionRequestRules(ctx, applicationId, versionId).RequestPhaseRuleRequest(requestPhaseRuleRequest).Execute()

Create an Application Request Rule



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
	requestPhaseRuleRequest := *openapiclient.NewRequestPhaseRuleRequest("Name_example", [][]ApplicationCriterionFieldRequest{[]openapiclient.ApplicationCriterionFieldRequest{*openapiclient.NewApplicationCriterionFieldRequest("Conditional_example", "Variable_example", "Operator_example")}}, []openapiclient.RequestPhaseBehaviorRequest{openapiclient.RequestPhaseBehaviorRequest{BehaviorArgs: openapiclient.NewBehaviorArgs("Type_example", *openapiclient.NewBehaviorArgsAttributes(*openapiclient.NewBehaviorArgsAttributesValue()))}}) // RequestPhaseRuleRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsRequestRulesAPI.CreateApplicationVersionRequestRules(context.Background(), applicationId, versionId).RequestPhaseRuleRequest(requestPhaseRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsRequestRulesAPI.CreateApplicationVersionRequestRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateApplicationVersionRequestRules`: RequestPhaseRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsRequestRulesAPI.CreateApplicationVersionRequestRules`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateApplicationVersionRequestRulesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **requestPhaseRuleRequest** | [**RequestPhaseRuleRequest**](RequestPhaseRuleRequest.md) |  | 

### Return type

[**RequestPhaseRuleResponse**](RequestPhaseRuleResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteApplicationRequestRule

> DeleteResponse DeleteApplicationRequestRule(ctx, applicationId, requestRuleId).Execute()

Delete an Application Request Rule



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
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsRequestRulesAPI.DeleteApplicationRequestRule(context.Background(), applicationId, requestRuleId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsRequestRulesAPI.DeleteApplicationRequestRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteApplicationRequestRule`: DeleteResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsRequestRulesAPI.DeleteApplicationRequestRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteApplicationRequestRuleRequest struct via the builder pattern


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


## DeleteApplicationVersionRequestRule

> DeleteResponse DeleteApplicationVersionRequestRule(ctx, applicationId, requestRuleId, versionId).Execute()

Delete an Application Request Rule



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
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.
	versionId := "versionId_example" // string | The ULID identifier of the version.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsRequestRulesAPI.DeleteApplicationVersionRequestRule(context.Background(), applicationId, requestRuleId, versionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsRequestRulesAPI.DeleteApplicationVersionRequestRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteApplicationVersionRequestRule`: DeleteResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsRequestRulesAPI.DeleteApplicationVersionRequestRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteApplicationVersionRequestRuleRequest struct via the builder pattern


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


## ListApplicationRequestRules

> PaginatedRequestPhaseRuleList ListApplicationRequestRules(ctx, applicationId).Description(description).Fields(fields).Id(id).LastEditor(lastEditor).LastModifiedGte(lastModifiedGte).LastModifiedLte(lastModifiedLte).Name(name).OrderGte(orderGte).OrderLte(orderLte).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()

List Application Request Rules



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
	applicationId := int64(789) // int64 | A unique integer value identifying the application.
	description := "description_example" // string | Filter by description (case-insensitive, partial match). (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	id := int64(789) // int64 | Filter by id (accepts comma-separated values). (optional)
	lastEditor := "lastEditor_example" // string | Filter by last editor (case-insensitive, partial match). (optional)
	lastModifiedGte := time.Now() // time.Time | Filter by last modified date (greater than or equal). (optional)
	lastModifiedLte := time.Now() // time.Time | Filter by last modified date (less than or equal). (optional)
	name := "name_example" // string | Filter by name (case-insensitive, partial match). (optional)
	orderGte := int64(789) // int64 | Filter by order (greater than or equal). (optional)
	orderLte := int64(789) // int64 | Filter by order (less than or equal). (optional)
	ordering := "ordering_example" // string | Which field to use when ordering the results. (Valid fields: id, name, description, last_editor, last_modified, order) (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	search := "search_example" // string | A search term to filter results. Searches across the following fields: name. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsRequestRulesAPI.ListApplicationRequestRules(context.Background(), applicationId).Description(description).Fields(fields).Id(id).LastEditor(lastEditor).LastModifiedGte(lastModifiedGte).LastModifiedLte(lastModifiedLte).Name(name).OrderGte(orderGte).OrderLte(orderLte).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsRequestRulesAPI.ListApplicationRequestRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListApplicationRequestRules`: PaginatedRequestPhaseRuleList
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsRequestRulesAPI.ListApplicationRequestRules`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListApplicationRequestRulesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **description** | **string** | Filter by description (case-insensitive, partial match). | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **id** | **int64** | Filter by id (accepts comma-separated values). | 
 **lastEditor** | **string** | Filter by last editor (case-insensitive, partial match). | 
 **lastModifiedGte** | **time.Time** | Filter by last modified date (greater than or equal). | 
 **lastModifiedLte** | **time.Time** | Filter by last modified date (less than or equal). | 
 **name** | **string** | Filter by name (case-insensitive, partial match). | 
 **orderGte** | **int64** | Filter by order (greater than or equal). | 
 **orderLte** | **int64** | Filter by order (less than or equal). | 
 **ordering** | **string** | Which field to use when ordering the results. (Valid fields: id, name, description, last_editor, last_modified, order) | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **search** | **string** | A search term to filter results. Searches across the following fields: name. | 

### Return type

[**PaginatedRequestPhaseRuleList**](PaginatedRequestPhaseRuleList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListApplicationVersionRequestRules

> PaginatedRequestPhaseRuleList ListApplicationVersionRequestRules(ctx, applicationId, versionId).Description(description).Fields(fields).Id(id).LastEditor(lastEditor).LastModifiedGte(lastModifiedGte).LastModifiedLte(lastModifiedLte).Name(name).OrderGte(orderGte).OrderLte(orderLte).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()

List Application Request Rules



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
	applicationId := int64(789) // int64 | A unique integer value identifying the application.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	description := "description_example" // string | Filter by description (case-insensitive, partial match). (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	id := int64(789) // int64 | Filter by id (accepts comma-separated values). (optional)
	lastEditor := "lastEditor_example" // string | Filter by last editor (case-insensitive, partial match). (optional)
	lastModifiedGte := time.Now() // time.Time | Filter by last modified date (greater than or equal). (optional)
	lastModifiedLte := time.Now() // time.Time | Filter by last modified date (less than or equal). (optional)
	name := "name_example" // string | Filter by name (case-insensitive, partial match). (optional)
	orderGte := int64(789) // int64 | Filter by order (greater than or equal). (optional)
	orderLte := int64(789) // int64 | Filter by order (less than or equal). (optional)
	ordering := "ordering_example" // string | Which field to use when ordering the results. (Valid fields: id, name, description, last_editor, last_modified, order) (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	search := "search_example" // string | A search term to filter results. Searches across the following fields: name. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsRequestRulesAPI.ListApplicationVersionRequestRules(context.Background(), applicationId, versionId).Description(description).Fields(fields).Id(id).LastEditor(lastEditor).LastModifiedGte(lastModifiedGte).LastModifiedLte(lastModifiedLte).Name(name).OrderGte(orderGte).OrderLte(orderLte).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsRequestRulesAPI.ListApplicationVersionRequestRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListApplicationVersionRequestRules`: PaginatedRequestPhaseRuleList
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsRequestRulesAPI.ListApplicationVersionRequestRules`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListApplicationVersionRequestRulesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **description** | **string** | Filter by description (case-insensitive, partial match). | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **id** | **int64** | Filter by id (accepts comma-separated values). | 
 **lastEditor** | **string** | Filter by last editor (case-insensitive, partial match). | 
 **lastModifiedGte** | **time.Time** | Filter by last modified date (greater than or equal). | 
 **lastModifiedLte** | **time.Time** | Filter by last modified date (less than or equal). | 
 **name** | **string** | Filter by name (case-insensitive, partial match). | 
 **orderGte** | **int64** | Filter by order (greater than or equal). | 
 **orderLte** | **int64** | Filter by order (less than or equal). | 
 **ordering** | **string** | Which field to use when ordering the results. (Valid fields: id, name, description, last_editor, last_modified, order) | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **search** | **string** | A search term to filter results. Searches across the following fields: name. | 

### Return type

[**PaginatedRequestPhaseRuleList**](PaginatedRequestPhaseRuleList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateApplicationRequestRule

> RequestPhaseRuleResponse PartialUpdateApplicationRequestRule(ctx, applicationId, requestRuleId).PatchedRequestPhaseRuleRequest(patchedRequestPhaseRuleRequest).Execute()

Partially update an Application Request Rule



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
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.
	patchedRequestPhaseRuleRequest := *openapiclient.NewPatchedRequestPhaseRuleRequest() // PatchedRequestPhaseRuleRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsRequestRulesAPI.PartialUpdateApplicationRequestRule(context.Background(), applicationId, requestRuleId).PatchedRequestPhaseRuleRequest(patchedRequestPhaseRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsRequestRulesAPI.PartialUpdateApplicationRequestRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateApplicationRequestRule`: RequestPhaseRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsRequestRulesAPI.PartialUpdateApplicationRequestRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateApplicationRequestRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **patchedRequestPhaseRuleRequest** | [**PatchedRequestPhaseRuleRequest**](PatchedRequestPhaseRuleRequest.md) |  | 

### Return type

[**RequestPhaseRuleResponse**](RequestPhaseRuleResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateApplicationVersionRequestRule

> RequestPhaseRuleResponse PartialUpdateApplicationVersionRequestRule(ctx, applicationId, requestRuleId, versionId).PatchedRequestPhaseRuleRequest(patchedRequestPhaseRuleRequest).Execute()

Partially update an Application Request Rule



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
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	patchedRequestPhaseRuleRequest := *openapiclient.NewPatchedRequestPhaseRuleRequest() // PatchedRequestPhaseRuleRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsRequestRulesAPI.PartialUpdateApplicationVersionRequestRule(context.Background(), applicationId, requestRuleId, versionId).PatchedRequestPhaseRuleRequest(patchedRequestPhaseRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsRequestRulesAPI.PartialUpdateApplicationVersionRequestRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateApplicationVersionRequestRule`: RequestPhaseRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsRequestRulesAPI.PartialUpdateApplicationVersionRequestRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateApplicationVersionRequestRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **patchedRequestPhaseRuleRequest** | [**PatchedRequestPhaseRuleRequest**](PatchedRequestPhaseRuleRequest.md) |  | 

### Return type

[**RequestPhaseRuleResponse**](RequestPhaseRuleResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveApplicationRequestRule

> ResponsePhaseRuleRetrieveResponse RetrieveApplicationRequestRule(ctx, applicationId, requestRuleId).Fields(fields).Execute()

Retrieve details of an Application Request Rule



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
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsRequestRulesAPI.RetrieveApplicationRequestRule(context.Background(), applicationId, requestRuleId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsRequestRulesAPI.RetrieveApplicationRequestRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveApplicationRequestRule`: ResponsePhaseRuleRetrieveResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsRequestRulesAPI.RetrieveApplicationRequestRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveApplicationRequestRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**ResponsePhaseRuleRetrieveResponse**](ResponsePhaseRuleRetrieveResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveApplicationVersionRequestRule

> ResponsePhaseRuleRetrieveResponse RetrieveApplicationVersionRequestRule(ctx, applicationId, requestRuleId, versionId).Fields(fields).Execute()

Retrieve details of an Application Request Rule



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
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsRequestRulesAPI.RetrieveApplicationVersionRequestRule(context.Background(), applicationId, requestRuleId, versionId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsRequestRulesAPI.RetrieveApplicationVersionRequestRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveApplicationVersionRequestRule`: ResponsePhaseRuleRetrieveResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsRequestRulesAPI.RetrieveApplicationVersionRequestRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveApplicationVersionRequestRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**ResponsePhaseRuleRetrieveResponse**](ResponsePhaseRuleRetrieveResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateApplicationRequestRule

> RequestPhaseRuleResponse UpdateApplicationRequestRule(ctx, applicationId, requestRuleId).RequestPhaseRuleRequest(requestPhaseRuleRequest).Execute()

Update an Application Request Rule



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
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.
	requestPhaseRuleRequest := *openapiclient.NewRequestPhaseRuleRequest("Name_example", [][]ApplicationCriterionFieldRequest{[]openapiclient.ApplicationCriterionFieldRequest{*openapiclient.NewApplicationCriterionFieldRequest("Conditional_example", "Variable_example", "Operator_example")}}, []openapiclient.RequestPhaseBehaviorRequest{openapiclient.RequestPhaseBehaviorRequest{BehaviorArgs: openapiclient.NewBehaviorArgs("Type_example", *openapiclient.NewBehaviorArgsAttributes(*openapiclient.NewBehaviorArgsAttributesValue()))}}) // RequestPhaseRuleRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsRequestRulesAPI.UpdateApplicationRequestRule(context.Background(), applicationId, requestRuleId).RequestPhaseRuleRequest(requestPhaseRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsRequestRulesAPI.UpdateApplicationRequestRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateApplicationRequestRule`: RequestPhaseRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsRequestRulesAPI.UpdateApplicationRequestRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateApplicationRequestRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **requestPhaseRuleRequest** | [**RequestPhaseRuleRequest**](RequestPhaseRuleRequest.md) |  | 

### Return type

[**RequestPhaseRuleResponse**](RequestPhaseRuleResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateApplicationRequestRulesOrder

> PaginatedRequestPhaseRuleList UpdateApplicationRequestRulesOrder(ctx, applicationId).ApplicationRequestPhaseRuleEngineOrderRequest(applicationRequestPhaseRuleEngineOrderRequest).Search(search).Execute()

Ordering Application Request Rules



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
	applicationRequestPhaseRuleEngineOrderRequest := *openapiclient.NewApplicationRequestPhaseRuleEngineOrderRequest([]int64{int64(123)}) // ApplicationRequestPhaseRuleEngineOrderRequest | 
	search := "search_example" // string | A search term to filter results. Searches across the following fields: name. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsRequestRulesAPI.UpdateApplicationRequestRulesOrder(context.Background(), applicationId).ApplicationRequestPhaseRuleEngineOrderRequest(applicationRequestPhaseRuleEngineOrderRequest).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsRequestRulesAPI.UpdateApplicationRequestRulesOrder``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateApplicationRequestRulesOrder`: PaginatedRequestPhaseRuleList
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsRequestRulesAPI.UpdateApplicationRequestRulesOrder`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateApplicationRequestRulesOrderRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **applicationRequestPhaseRuleEngineOrderRequest** | [**ApplicationRequestPhaseRuleEngineOrderRequest**](ApplicationRequestPhaseRuleEngineOrderRequest.md) |  | 
 **search** | **string** | A search term to filter results. Searches across the following fields: name. | 

### Return type

[**PaginatedRequestPhaseRuleList**](PaginatedRequestPhaseRuleList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateApplicationVersionRequestRule

> RequestPhaseRuleResponse UpdateApplicationVersionRequestRule(ctx, applicationId, requestRuleId, versionId).RequestPhaseRuleRequest(requestPhaseRuleRequest).Execute()

Update an Application Request Rule



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
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	requestPhaseRuleRequest := *openapiclient.NewRequestPhaseRuleRequest("Name_example", [][]ApplicationCriterionFieldRequest{[]openapiclient.ApplicationCriterionFieldRequest{*openapiclient.NewApplicationCriterionFieldRequest("Conditional_example", "Variable_example", "Operator_example")}}, []openapiclient.RequestPhaseBehaviorRequest{openapiclient.RequestPhaseBehaviorRequest{BehaviorArgs: openapiclient.NewBehaviorArgs("Type_example", *openapiclient.NewBehaviorArgsAttributes(*openapiclient.NewBehaviorArgsAttributesValue()))}}) // RequestPhaseRuleRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsRequestRulesAPI.UpdateApplicationVersionRequestRule(context.Background(), applicationId, requestRuleId, versionId).RequestPhaseRuleRequest(requestPhaseRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsRequestRulesAPI.UpdateApplicationVersionRequestRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateApplicationVersionRequestRule`: RequestPhaseRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsRequestRulesAPI.UpdateApplicationVersionRequestRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateApplicationVersionRequestRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **requestPhaseRuleRequest** | [**RequestPhaseRuleRequest**](RequestPhaseRuleRequest.md) |  | 

### Return type

[**RequestPhaseRuleResponse**](RequestPhaseRuleResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateApplicationVersionRequestRulesOrder

> PaginatedRequestPhaseRuleList UpdateApplicationVersionRequestRulesOrder(ctx, applicationId, versionId).ApplicationRequestPhaseRuleEngineOrderRequest(applicationRequestPhaseRuleEngineOrderRequest).Search(search).Execute()

Ordering Application Request Rules



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
	applicationRequestPhaseRuleEngineOrderRequest := *openapiclient.NewApplicationRequestPhaseRuleEngineOrderRequest([]int64{int64(123)}) // ApplicationRequestPhaseRuleEngineOrderRequest | 
	search := "search_example" // string | A search term to filter results. Searches across the following fields: name. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ApplicationsRequestRulesAPI.UpdateApplicationVersionRequestRulesOrder(context.Background(), applicationId, versionId).ApplicationRequestPhaseRuleEngineOrderRequest(applicationRequestPhaseRuleEngineOrderRequest).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ApplicationsRequestRulesAPI.UpdateApplicationVersionRequestRulesOrder``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateApplicationVersionRequestRulesOrder`: PaginatedRequestPhaseRuleList
	fmt.Fprintf(os.Stdout, "Response from `ApplicationsRequestRulesAPI.UpdateApplicationVersionRequestRulesOrder`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**applicationId** | **int64** | A unique integer value identifying the application. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateApplicationVersionRequestRulesOrderRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **applicationRequestPhaseRuleEngineOrderRequest** | [**ApplicationRequestPhaseRuleEngineOrderRequest**](ApplicationRequestPhaseRuleEngineOrderRequest.md) |  | 
 **search** | **string** | A search term to filter results. Searches across the following fields: name. | 

### Return type

[**PaginatedRequestPhaseRuleList**](PaginatedRequestPhaseRuleList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

