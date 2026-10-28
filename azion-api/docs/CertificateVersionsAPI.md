# \CertificateVersionsAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListCertificateVersions**](CertificateVersionsAPI.md#ListCertificateVersions) | **Get** /workspace/tls/certificates/{resource_pk}/versions | List certificate versions
[**RetrieveCertificateVersion**](CertificateVersionsAPI.md#RetrieveCertificateVersion) | **Get** /workspace/tls/certificates/{resource_pk}/versions/{id} | Retrieve a certificate version
[**RevertCertificateVersion**](CertificateVersionsAPI.md#RevertCertificateVersion) | **Post** /workspace/tls/certificates/{resource_pk}/versions/{id}/revert | Revert to a certificate version



## ListCertificateVersions

> PaginatedCertificateList ListCertificateVersions(ctx, resourcePk).Fields(fields).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()

List certificate versions



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
	resourcePk := int64(789) // int64 | The ID of the certificate resource.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	ordering := "ordering_example" // string | Which field to use when ordering the results. (optional)
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)
	search := "search_example" // string | A search term. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CertificateVersionsAPI.ListCertificateVersions(context.Background(), resourcePk).Fields(fields).Ordering(ordering).Page(page).PageSize(pageSize).Search(search).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CertificateVersionsAPI.ListCertificateVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCertificateVersions`: PaginatedCertificateList
	fmt.Fprintf(os.Stdout, "Response from `CertificateVersionsAPI.ListCertificateVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**resourcePk** | **int64** | The ID of the certificate resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListCertificateVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **ordering** | **string** | Which field to use when ordering the results. | 
 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 
 **search** | **string** | A search term. | 

### Return type

[**PaginatedCertificateList**](PaginatedCertificateList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveCertificateVersion

> Certificate RetrieveCertificateVersion(ctx, id, resourcePk).Fields(fields).Execute()

Retrieve a certificate version



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
	resourcePk := int64(789) // int64 | The ID of the certificate resource.
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CertificateVersionsAPI.RetrieveCertificateVersion(context.Background(), id, resourcePk).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CertificateVersionsAPI.RetrieveCertificateVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveCertificateVersion`: Certificate
	fmt.Fprintf(os.Stdout, "Response from `CertificateVersionsAPI.RetrieveCertificateVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | The ULID identifier of the version. | 
**resourcePk** | **int64** | The ID of the certificate resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveCertificateVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**Certificate**](Certificate.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RevertCertificateVersion

> RevertCertificateVersion(ctx, id, resourcePk).VersionRevert(versionRevert).Execute()

Revert to a certificate version



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
	resourcePk := int64(789) // int64 | The ID of the certificate resource.
	versionRevert := *openapiclient.NewVersionRevert() // VersionRevert |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CertificateVersionsAPI.RevertCertificateVersion(context.Background(), id, resourcePk).VersionRevert(versionRevert).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CertificateVersionsAPI.RevertCertificateVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | The ULID identifier of the version. | 
**resourcePk** | **int64** | The ID of the certificate resource. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRevertCertificateVersionRequest struct via the builder pattern


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

