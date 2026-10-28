# \FirewallsRulesEngineAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateFirewallRule**](FirewallsRulesEngineAPI.md#CreateFirewallRule) | **Post** /workspace/firewalls/{firewall_id}/request_rules | Create an Firewall Rule
[**CreateFirewallVersionRequestRules**](FirewallsRulesEngineAPI.md#CreateFirewallVersionRequestRules) | **Post** /workspace/firewalls/{firewall_id}/versions/{version_id}/request_rules | Create an Firewall Rule
[**DeleteFirewallRule**](FirewallsRulesEngineAPI.md#DeleteFirewallRule) | **Delete** /workspace/firewalls/{firewall_id}/request_rules/{request_rule_id} | Delete an Firewall Rule
[**DeleteFirewallVersionRequestRule**](FirewallsRulesEngineAPI.md#DeleteFirewallVersionRequestRule) | **Delete** /workspace/firewalls/{firewall_id}/versions/{version_id}/request_rules/{request_rule_id} | Delete an Firewall Rule
[**ListFirewallRules**](FirewallsRulesEngineAPI.md#ListFirewallRules) | **Get** /workspace/firewalls/{firewall_id}/request_rules | List Firewall Rules
[**ListFirewallVersionRequestRules**](FirewallsRulesEngineAPI.md#ListFirewallVersionRequestRules) | **Get** /workspace/firewalls/{firewall_id}/versions/{version_id}/request_rules | List Firewall Rules
[**OrderFirewallRules**](FirewallsRulesEngineAPI.md#OrderFirewallRules) | **Put** /workspace/firewalls/{firewall_id}/request_rules/order | Ordering Firewall Rules
[**PartialUpdateFirewallRule**](FirewallsRulesEngineAPI.md#PartialUpdateFirewallRule) | **Patch** /workspace/firewalls/{firewall_id}/request_rules/{request_rule_id} | Partially update an Firewall Rule
[**PartialUpdateFirewallVersionRequestRule**](FirewallsRulesEngineAPI.md#PartialUpdateFirewallVersionRequestRule) | **Patch** /workspace/firewalls/{firewall_id}/versions/{version_id}/request_rules/{request_rule_id} | Partially update an Firewall Rule
[**RetrieveFirewallRule**](FirewallsRulesEngineAPI.md#RetrieveFirewallRule) | **Get** /workspace/firewalls/{firewall_id}/request_rules/{request_rule_id} | Retrieve details of an Firewall Rule
[**RetrieveFirewallVersionRequestRule**](FirewallsRulesEngineAPI.md#RetrieveFirewallVersionRequestRule) | **Get** /workspace/firewalls/{firewall_id}/versions/{version_id}/request_rules/{request_rule_id} | Retrieve details of an Firewall Rule
[**UpdateFirewallRule**](FirewallsRulesEngineAPI.md#UpdateFirewallRule) | **Put** /workspace/firewalls/{firewall_id}/request_rules/{request_rule_id} | Update an Firewall Rule
[**UpdateFirewallVersionRequestRule**](FirewallsRulesEngineAPI.md#UpdateFirewallVersionRequestRule) | **Put** /workspace/firewalls/{firewall_id}/versions/{version_id}/request_rules/{request_rule_id} | Update an Firewall Rule
[**UpdateFirewallVersionRequestRulesOrder**](FirewallsRulesEngineAPI.md#UpdateFirewallVersionRequestRulesOrder) | **Put** /workspace/firewalls/{firewall_id}/versions/{version_id}/request_rules/order | Ordering Firewall Rules



## CreateFirewallRule

> FirewallRuleResponse CreateFirewallRule(ctx, firewallId).FirewallRuleRequest(firewallRuleRequest).Execute()

Create an Firewall Rule



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
	firewallId := int64(789) // int64 | A unique integer value identifying the firewall.
	firewallRuleRequest := *openapiclient.NewFirewallRuleRequest("Name_example", [][]FirewallCriterionFieldRequest{[]openapiclient.FirewallCriterionFieldRequest{*openapiclient.NewFirewallCriterionFieldRequest("Conditional_example", "Variable_example", "Operator_example")}}, []openapiclient.FirewallBehaviorRequest{openapiclient.FirewallBehaviorRequest{FirewallBehaviorArgsRequest: openapiclient.NewFirewallBehaviorArgsRequest("Type_example", *openapiclient.NewFirewallBehaviorRunFunctionAttributesRequest(int64(123)))}}) // FirewallRuleRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallsRulesEngineAPI.CreateFirewallRule(context.Background(), firewallId).FirewallRuleRequest(firewallRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallsRulesEngineAPI.CreateFirewallRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateFirewallRule`: FirewallRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `FirewallsRulesEngineAPI.CreateFirewallRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | A unique integer value identifying the firewall. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateFirewallRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **firewallRuleRequest** | [**FirewallRuleRequest**](FirewallRuleRequest.md) |  | 

### Return type

[**FirewallRuleResponse**](FirewallRuleResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateFirewallVersionRequestRules

> FirewallRuleResponse CreateFirewallVersionRequestRules(ctx, firewallId, versionId).FirewallRuleRequest(firewallRuleRequest).Execute()

Create an Firewall Rule



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
	firewallId := int64(789) // int64 | A unique integer value identifying the firewall.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	firewallRuleRequest := *openapiclient.NewFirewallRuleRequest("Name_example", [][]FirewallCriterionFieldRequest{[]openapiclient.FirewallCriterionFieldRequest{*openapiclient.NewFirewallCriterionFieldRequest("Conditional_example", "Variable_example", "Operator_example")}}, []openapiclient.FirewallBehaviorRequest{openapiclient.FirewallBehaviorRequest{FirewallBehaviorArgsRequest: openapiclient.NewFirewallBehaviorArgsRequest("Type_example", *openapiclient.NewFirewallBehaviorRunFunctionAttributesRequest(int64(123)))}}) // FirewallRuleRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallsRulesEngineAPI.CreateFirewallVersionRequestRules(context.Background(), firewallId, versionId).FirewallRuleRequest(firewallRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallsRulesEngineAPI.CreateFirewallVersionRequestRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateFirewallVersionRequestRules`: FirewallRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `FirewallsRulesEngineAPI.CreateFirewallVersionRequestRules`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | A unique integer value identifying the firewall. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateFirewallVersionRequestRulesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **firewallRuleRequest** | [**FirewallRuleRequest**](FirewallRuleRequest.md) |  | 

### Return type

[**FirewallRuleResponse**](FirewallRuleResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteFirewallRule

> DeleteResponse DeleteFirewallRule(ctx, firewallId, requestRuleId).Execute()

Delete an Firewall Rule



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
	firewallId := int64(789) // int64 | A unique integer value identifying the firewall.
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallsRulesEngineAPI.DeleteFirewallRule(context.Background(), firewallId, requestRuleId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallsRulesEngineAPI.DeleteFirewallRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteFirewallRule`: DeleteResponse
	fmt.Fprintf(os.Stdout, "Response from `FirewallsRulesEngineAPI.DeleteFirewallRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | A unique integer value identifying the firewall. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteFirewallRuleRequest struct via the builder pattern


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


## DeleteFirewallVersionRequestRule

> DeleteResponse DeleteFirewallVersionRequestRule(ctx, firewallId, requestRuleId, versionId).Execute()

Delete an Firewall Rule



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
	firewallId := int64(789) // int64 | A unique integer value identifying the firewall.
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.
	versionId := "versionId_example" // string | The ULID identifier of the version.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallsRulesEngineAPI.DeleteFirewallVersionRequestRule(context.Background(), firewallId, requestRuleId, versionId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallsRulesEngineAPI.DeleteFirewallVersionRequestRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteFirewallVersionRequestRule`: DeleteResponse
	fmt.Fprintf(os.Stdout, "Response from `FirewallsRulesEngineAPI.DeleteFirewallVersionRequestRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | A unique integer value identifying the firewall. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteFirewallVersionRequestRuleRequest struct via the builder pattern


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


## ListFirewallRules

> PaginatedFirewallRuleList ListFirewallRules(ctx, firewallId).Description(description).Fields(fields).Id(id).LastEditor(lastEditor).LastModifiedGte(lastModifiedGte).LastModifiedLte(lastModifiedLte).Name(name).OrderGte(orderGte).OrderLte(orderLte).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()

List Firewall Rules



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
	firewallId := int64(789) // int64 | A unique integer value identifying the firewall.
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
	search := "search_example" // string | A search term to filter results. Searches across the following fields: name, last_editor. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallsRulesEngineAPI.ListFirewallRules(context.Background(), firewallId).Description(description).Fields(fields).Id(id).LastEditor(lastEditor).LastModifiedGte(lastModifiedGte).LastModifiedLte(lastModifiedLte).Name(name).OrderGte(orderGte).OrderLte(orderLte).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallsRulesEngineAPI.ListFirewallRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListFirewallRules`: PaginatedFirewallRuleList
	fmt.Fprintf(os.Stdout, "Response from `FirewallsRulesEngineAPI.ListFirewallRules`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | A unique integer value identifying the firewall. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListFirewallRulesRequest struct via the builder pattern


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
 **search** | **string** | A search term to filter results. Searches across the following fields: name, last_editor. | 

### Return type

[**PaginatedFirewallRuleList**](PaginatedFirewallRuleList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListFirewallVersionRequestRules

> PaginatedFirewallRuleList ListFirewallVersionRequestRules(ctx, firewallId, versionId).Description(description).Fields(fields).Id(id).LastEditor(lastEditor).LastModifiedGte(lastModifiedGte).LastModifiedLte(lastModifiedLte).Name(name).OrderGte(orderGte).OrderLte(orderLte).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()

List Firewall Rules



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
	firewallId := int64(789) // int64 | A unique integer value identifying the firewall.
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
	search := "search_example" // string | A search term to filter results. Searches across the following fields: name, last_editor. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallsRulesEngineAPI.ListFirewallVersionRequestRules(context.Background(), firewallId, versionId).Description(description).Fields(fields).Id(id).LastEditor(lastEditor).LastModifiedGte(lastModifiedGte).LastModifiedLte(lastModifiedLte).Name(name).OrderGte(orderGte).OrderLte(orderLte).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallsRulesEngineAPI.ListFirewallVersionRequestRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListFirewallVersionRequestRules`: PaginatedFirewallRuleList
	fmt.Fprintf(os.Stdout, "Response from `FirewallsRulesEngineAPI.ListFirewallVersionRequestRules`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | A unique integer value identifying the firewall. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListFirewallVersionRequestRulesRequest struct via the builder pattern


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
 **search** | **string** | A search term to filter results. Searches across the following fields: name, last_editor. | 

### Return type

[**PaginatedFirewallRuleList**](PaginatedFirewallRuleList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## OrderFirewallRules

> PaginatedFirewallRuleList OrderFirewallRules(ctx, firewallId).FirewallRuleEngineOrderRequest(firewallRuleEngineOrderRequest).Search(search).Execute()

Ordering Firewall Rules



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
	firewallId := int64(789) // int64 | A unique integer value identifying the firewall.
	firewallRuleEngineOrderRequest := *openapiclient.NewFirewallRuleEngineOrderRequest([]int64{int64(123)}) // FirewallRuleEngineOrderRequest | 
	search := "search_example" // string | A search term to filter results. Searches across the following fields: name, last_editor. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallsRulesEngineAPI.OrderFirewallRules(context.Background(), firewallId).FirewallRuleEngineOrderRequest(firewallRuleEngineOrderRequest).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallsRulesEngineAPI.OrderFirewallRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `OrderFirewallRules`: PaginatedFirewallRuleList
	fmt.Fprintf(os.Stdout, "Response from `FirewallsRulesEngineAPI.OrderFirewallRules`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | A unique integer value identifying the firewall. | 

### Other Parameters

Other parameters are passed through a pointer to a apiOrderFirewallRulesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **firewallRuleEngineOrderRequest** | [**FirewallRuleEngineOrderRequest**](FirewallRuleEngineOrderRequest.md) |  | 
 **search** | **string** | A search term to filter results. Searches across the following fields: name, last_editor. | 

### Return type

[**PaginatedFirewallRuleList**](PaginatedFirewallRuleList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateFirewallRule

> FirewallRuleResponse PartialUpdateFirewallRule(ctx, firewallId, requestRuleId).PatchedFirewallRuleRequest(patchedFirewallRuleRequest).Execute()

Partially update an Firewall Rule



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
	firewallId := int64(789) // int64 | A unique integer value identifying the firewall.
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.
	patchedFirewallRuleRequest := *openapiclient.NewPatchedFirewallRuleRequest() // PatchedFirewallRuleRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallsRulesEngineAPI.PartialUpdateFirewallRule(context.Background(), firewallId, requestRuleId).PatchedFirewallRuleRequest(patchedFirewallRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallsRulesEngineAPI.PartialUpdateFirewallRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateFirewallRule`: FirewallRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `FirewallsRulesEngineAPI.PartialUpdateFirewallRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | A unique integer value identifying the firewall. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateFirewallRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **patchedFirewallRuleRequest** | [**PatchedFirewallRuleRequest**](PatchedFirewallRuleRequest.md) |  | 

### Return type

[**FirewallRuleResponse**](FirewallRuleResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PartialUpdateFirewallVersionRequestRule

> FirewallRuleResponse PartialUpdateFirewallVersionRequestRule(ctx, firewallId, requestRuleId, versionId).PatchedFirewallRuleRequest(patchedFirewallRuleRequest).Execute()

Partially update an Firewall Rule



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
	firewallId := int64(789) // int64 | A unique integer value identifying the firewall.
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	patchedFirewallRuleRequest := *openapiclient.NewPatchedFirewallRuleRequest() // PatchedFirewallRuleRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallsRulesEngineAPI.PartialUpdateFirewallVersionRequestRule(context.Background(), firewallId, requestRuleId, versionId).PatchedFirewallRuleRequest(patchedFirewallRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallsRulesEngineAPI.PartialUpdateFirewallVersionRequestRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PartialUpdateFirewallVersionRequestRule`: FirewallRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `FirewallsRulesEngineAPI.PartialUpdateFirewallVersionRequestRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | A unique integer value identifying the firewall. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiPartialUpdateFirewallVersionRequestRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **patchedFirewallRuleRequest** | [**PatchedFirewallRuleRequest**](PatchedFirewallRuleRequest.md) |  | 

### Return type

[**FirewallRuleResponse**](FirewallRuleResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveFirewallRule

> FirewallRuleRetrieveResponse RetrieveFirewallRule(ctx, firewallId, requestRuleId).Fields(fields).Execute()

Retrieve details of an Firewall Rule



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
	firewallId := int64(789) // int64 | A unique integer value identifying the firewall.
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallsRulesEngineAPI.RetrieveFirewallRule(context.Background(), firewallId, requestRuleId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallsRulesEngineAPI.RetrieveFirewallRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveFirewallRule`: FirewallRuleRetrieveResponse
	fmt.Fprintf(os.Stdout, "Response from `FirewallsRulesEngineAPI.RetrieveFirewallRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | A unique integer value identifying the firewall. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveFirewallRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**FirewallRuleRetrieveResponse**](FirewallRuleRetrieveResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveFirewallVersionRequestRule

> FirewallRuleRetrieveResponse RetrieveFirewallVersionRequestRule(ctx, firewallId, requestRuleId, versionId).Fields(fields).Execute()

Retrieve details of an Firewall Rule



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
	firewallId := int64(789) // int64 | A unique integer value identifying the firewall.
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallsRulesEngineAPI.RetrieveFirewallVersionRequestRule(context.Background(), firewallId, requestRuleId, versionId).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallsRulesEngineAPI.RetrieveFirewallVersionRequestRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveFirewallVersionRequestRule`: FirewallRuleRetrieveResponse
	fmt.Fprintf(os.Stdout, "Response from `FirewallsRulesEngineAPI.RetrieveFirewallVersionRequestRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | A unique integer value identifying the firewall. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveFirewallVersionRequestRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**FirewallRuleRetrieveResponse**](FirewallRuleRetrieveResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateFirewallRule

> FirewallRuleResponse UpdateFirewallRule(ctx, firewallId, requestRuleId).FirewallRuleRequest(firewallRuleRequest).Execute()

Update an Firewall Rule



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
	firewallId := int64(789) // int64 | A unique integer value identifying the firewall.
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.
	firewallRuleRequest := *openapiclient.NewFirewallRuleRequest("Name_example", [][]FirewallCriterionFieldRequest{[]openapiclient.FirewallCriterionFieldRequest{*openapiclient.NewFirewallCriterionFieldRequest("Conditional_example", "Variable_example", "Operator_example")}}, []openapiclient.FirewallBehaviorRequest{openapiclient.FirewallBehaviorRequest{FirewallBehaviorArgsRequest: openapiclient.NewFirewallBehaviorArgsRequest("Type_example", *openapiclient.NewFirewallBehaviorRunFunctionAttributesRequest(int64(123)))}}) // FirewallRuleRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallsRulesEngineAPI.UpdateFirewallRule(context.Background(), firewallId, requestRuleId).FirewallRuleRequest(firewallRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallsRulesEngineAPI.UpdateFirewallRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateFirewallRule`: FirewallRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `FirewallsRulesEngineAPI.UpdateFirewallRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | A unique integer value identifying the firewall. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateFirewallRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **firewallRuleRequest** | [**FirewallRuleRequest**](FirewallRuleRequest.md) |  | 

### Return type

[**FirewallRuleResponse**](FirewallRuleResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateFirewallVersionRequestRule

> FirewallRuleResponse UpdateFirewallVersionRequestRule(ctx, firewallId, requestRuleId, versionId).FirewallRuleRequest(firewallRuleRequest).Execute()

Update an Firewall Rule



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
	firewallId := int64(789) // int64 | A unique integer value identifying the firewall.
	requestRuleId := int64(789) // int64 | A unique integer value identifying the request rule.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	firewallRuleRequest := *openapiclient.NewFirewallRuleRequest("Name_example", [][]FirewallCriterionFieldRequest{[]openapiclient.FirewallCriterionFieldRequest{*openapiclient.NewFirewallCriterionFieldRequest("Conditional_example", "Variable_example", "Operator_example")}}, []openapiclient.FirewallBehaviorRequest{openapiclient.FirewallBehaviorRequest{FirewallBehaviorArgsRequest: openapiclient.NewFirewallBehaviorArgsRequest("Type_example", *openapiclient.NewFirewallBehaviorRunFunctionAttributesRequest(int64(123)))}}) // FirewallRuleRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallsRulesEngineAPI.UpdateFirewallVersionRequestRule(context.Background(), firewallId, requestRuleId, versionId).FirewallRuleRequest(firewallRuleRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallsRulesEngineAPI.UpdateFirewallVersionRequestRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateFirewallVersionRequestRule`: FirewallRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `FirewallsRulesEngineAPI.UpdateFirewallVersionRequestRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | A unique integer value identifying the firewall. | 
**requestRuleId** | **int64** | A unique integer value identifying the request rule. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateFirewallVersionRequestRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **firewallRuleRequest** | [**FirewallRuleRequest**](FirewallRuleRequest.md) |  | 

### Return type

[**FirewallRuleResponse**](FirewallRuleResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateFirewallVersionRequestRulesOrder

> PaginatedFirewallRuleList UpdateFirewallVersionRequestRulesOrder(ctx, firewallId, versionId).FirewallRuleEngineOrderRequest(firewallRuleEngineOrderRequest).Search(search).Execute()

Ordering Firewall Rules



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
	firewallId := int64(789) // int64 | A unique integer value identifying the firewall.
	versionId := "versionId_example" // string | The ULID identifier of the version.
	firewallRuleEngineOrderRequest := *openapiclient.NewFirewallRuleEngineOrderRequest([]int64{int64(123)}) // FirewallRuleEngineOrderRequest | 
	search := "search_example" // string | A search term to filter results. Searches across the following fields: name, last_editor. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FirewallsRulesEngineAPI.UpdateFirewallVersionRequestRulesOrder(context.Background(), firewallId, versionId).FirewallRuleEngineOrderRequest(firewallRuleEngineOrderRequest).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FirewallsRulesEngineAPI.UpdateFirewallVersionRequestRulesOrder``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateFirewallVersionRequestRulesOrder`: PaginatedFirewallRuleList
	fmt.Fprintf(os.Stdout, "Response from `FirewallsRulesEngineAPI.UpdateFirewallVersionRequestRulesOrder`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**firewallId** | **int64** | A unique integer value identifying the firewall. | 
**versionId** | **string** | The ULID identifier of the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateFirewallVersionRequestRulesOrderRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **firewallRuleEngineOrderRequest** | [**FirewallRuleEngineOrderRequest**](FirewallRuleEngineOrderRequest.md) |  | 
 **search** | **string** | A search term to filter results. Searches across the following fields: name, last_editor. | 

### Return type

[**PaginatedFirewallRuleList**](PaginatedFirewallRuleList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

