# \CRLVersionsAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListCrlVersions**](CRLVersionsAPI.md#ListCrlVersions) | **Get** /workspace/tls/crls/{resource_pk}/versions | List CRL versions
[**RetrieveCrlVersion**](CRLVersionsAPI.md#RetrieveCrlVersion) | **Get** /workspace/tls/crls/{resource_pk}/versions/{id} | Retrieve a CRL version
[**RevertCrlVersion**](CRLVersionsAPI.md#RevertCrlVersion) | **Post** /workspace/tls/crls/{resource_pk}/versions/{id}/revert | Revert to a CRL version



## ListCrlVersions

> PaginatedCertificateRevocationList ListCrlVersions(ctx, resourcePk).Fields(fields).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()

List CRL versions



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
	resourcePk := int64(789) // int64 | The ID of the CRL resource.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	ordering := "ordering_example" // string | Which field to use when ordering the results. (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	search := "search_example" // string | A search term. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CRLVersionsAPI.ListCrlVersions(context.Background(), resourcePk).Fields(fields).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CRLVersionsAPI.ListCrlVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCrlVersions`: PaginatedCertificateRevocationList
	fmt.Fprintf(os.Stdout, "Response from `CRLVersionsAPI.ListCrlVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**resourcePk** | **int64** | The ID of the CRL resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListCrlVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **ordering** | **string** | Which field to use when ordering the results. | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **search** | **string** | A search term. | 

### Return type

[**PaginatedCertificateRevocationList**](PaginatedCertificateRevocationList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveCrlVersion

> CertificateRevocationList RetrieveCrlVersion(ctx, id, resourcePk).Fields(fields).Execute()

Retrieve a CRL version



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
	id := "id_example" // string | The ULID identifier of the version.
	resourcePk := int64(789) // int64 | The ID of the CRL resource.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CRLVersionsAPI.RetrieveCrlVersion(context.Background(), id, resourcePk).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CRLVersionsAPI.RetrieveCrlVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveCrlVersion`: CertificateRevocationList
	fmt.Fprintf(os.Stdout, "Response from `CRLVersionsAPI.RetrieveCrlVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | The ULID identifier of the version. | 
**resourcePk** | **int64** | The ID of the CRL resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveCrlVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**CertificateRevocationList**](CertificateRevocationList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RevertCrlVersion

> RevertCrlVersion(ctx, id, resourcePk).VersionRevert(versionRevert).Execute()

Revert to a CRL version



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
	id := "id_example" // string | The ULID identifier of the version.
	resourcePk := int64(789) // int64 | The ID of the CRL resource.
	versionRevert := *openapiclient.NewVersionRevert() // VersionRevert |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CRLVersionsAPI.RevertCrlVersion(context.Background(), id, resourcePk).VersionRevert(versionRevert).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CRLVersionsAPI.RevertCrlVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | The ULID identifier of the version. | 
**resourcePk** | **int64** | The ID of the CRL resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRevertCrlVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **versionRevert** | [**VersionRevert**](VersionRevert.md) |  | 

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

