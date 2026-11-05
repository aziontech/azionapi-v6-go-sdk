# \CRLVersionsAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListCrlVersions**](CRLVersionsAPI.md#ListCrlVersions) | **Get** /workspace/tls/crls/{crl_id}/versions | List CRL versions
[**RetrieveCrlVersion**](CRLVersionsAPI.md#RetrieveCrlVersion) | **Get** /workspace/tls/crls/{crl_id}/versions/{version_id} | Retrieve a CRL version
[**RevertCrlVersion**](CRLVersionsAPI.md#RevertCrlVersion) | **Post** /workspace/tls/crls/{crl_id}/versions/{version_id}/revert | Revert to a CRL version



## ListCrlVersions

> PaginatedCertificateRevocationListVersionList ListCrlVersions(ctx, crlId).Page(page).PageSize(pageSize).Execute()

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
	crlId := int64(789) // int64 | A unique value identifying the certificate revocation list.
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CRLVersionsAPI.ListCrlVersions(context.Background(), crlId).Page(page).PageSize(pageSize).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CRLVersionsAPI.ListCrlVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCrlVersions`: PaginatedCertificateRevocationListVersionList
	fmt.Fprintf(os.Stdout, "Response from `CRLVersionsAPI.ListCrlVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**crlId** | **int64** | A unique value identifying the certificate revocation list. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListCrlVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 

### Return type

[**PaginatedCertificateRevocationListVersionList**](PaginatedCertificateRevocationListVersionList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveCrlVersion

> CertificateRevocationListVersion RetrieveCrlVersion(ctx, crlId, versionId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()

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
	crlId := int64(789) // int64 | A unique value identifying the certificate revocation list.
	versionId := "versionId_example" // string | A unique value identifying the version.
	dependencies := true // bool | Include the resources this version references. (optional)
	dependencyStates := []string{"Inner_example"} // []string | Keep only the dependency versions in these states (comma-separated). Needs dependencies=true. (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CRLVersionsAPI.RetrieveCrlVersion(context.Background(), crlId, versionId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CRLVersionsAPI.RetrieveCrlVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveCrlVersion`: CertificateRevocationListVersion
	fmt.Fprintf(os.Stdout, "Response from `CRLVersionsAPI.RetrieveCrlVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**crlId** | **int64** | A unique value identifying the certificate revocation list. | 
**versionId** | **string** | A unique value identifying the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveCrlVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **dependencies** | **bool** | Include the resources this version references. | 
 **dependencyStates** | **[]string** | Keep only the dependency versions in these states (comma-separated). Needs dependencies&#x3D;true. | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**CertificateRevocationListVersion**](CertificateRevocationListVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RevertCrlVersion

> CertificateRevocationListVersionMeta RevertCrlVersion(ctx, crlId, versionId).CertificateRevocationListVersionRevertRequest(certificateRevocationListVersionRevertRequest).Execute()

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
	crlId := int64(789) // int64 | A unique value identifying the certificate revocation list.
	versionId := "versionId_example" // string | A unique value identifying the version.
	certificateRevocationListVersionRevertRequest := *openapiclient.NewCertificateRevocationListVersionRevertRequest() // CertificateRevocationListVersionRevertRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CRLVersionsAPI.RevertCrlVersion(context.Background(), crlId, versionId).CertificateRevocationListVersionRevertRequest(certificateRevocationListVersionRevertRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CRLVersionsAPI.RevertCrlVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RevertCrlVersion`: CertificateRevocationListVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `CRLVersionsAPI.RevertCrlVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**crlId** | **int64** | A unique value identifying the certificate revocation list. | 
**versionId** | **string** | A unique value identifying the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRevertCrlVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **certificateRevocationListVersionRevertRequest** | [**CertificateRevocationListVersionRevertRequest**](CertificateRevocationListVersionRevertRequest.md) |  | 

### Return type

[**CertificateRevocationListVersionMeta**](CertificateRevocationListVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

