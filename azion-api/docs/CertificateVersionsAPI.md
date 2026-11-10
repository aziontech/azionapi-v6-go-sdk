# \CertificateVersionsAPI

All URIs are relative to *https://stage-api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListCertificateVersions**](CertificateVersionsAPI.md#ListCertificateVersions) | **Get** /workspace/tls/certificates/{certificate_id}/versions | List certificate versions
[**RetrieveCertificateVersion**](CertificateVersionsAPI.md#RetrieveCertificateVersion) | **Get** /workspace/tls/certificates/{certificate_id}/versions/{version_id} | Retrieve a certificate version
[**RevertCertificateVersion**](CertificateVersionsAPI.md#RevertCertificateVersion) | **Post** /workspace/tls/certificates/{certificate_id}/versions/{version_id}/revert | Revert to a certificate version



## ListCertificateVersions

> PaginatedCertificateVersionList ListCertificateVersions(ctx, certificateId).Page(page).PageSize(pageSize).Execute()

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
	certificateId := int64(789) // int64 | A unique value identifying the certificate.
	page := int64(789) // int64 | A page number within the paginated result set. (optional)
	pageSize := int32(56) // int32 | A numeric value that indicates the number of items per page. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CertificateVersionsAPI.ListCertificateVersions(context.Background(), certificateId).Page(page).PageSize(pageSize).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CertificateVersionsAPI.ListCertificateVersions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCertificateVersions`: PaginatedCertificateVersionList
	fmt.Fprintf(os.Stdout, "Response from `CertificateVersionsAPI.ListCertificateVersions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**certificateId** | **int64** | A unique value identifying the certificate. | 

### Other Parameters

Other parameters are passed through a pointer to a apiListCertificateVersionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int64** | A page number within the paginated result set. | 
 **pageSize** | **int32** | A numeric value that indicates the number of items per page. | 

### Return type

[**PaginatedCertificateVersionList**](PaginatedCertificateVersionList.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveCertificateVersion

> CertificateVersion RetrieveCertificateVersion(ctx, certificateId, versionId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()

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
	certificateId := int64(789) // int64 | A unique value identifying the certificate.
	versionId := "versionId_example" // string | A unique value identifying the version.
	dependencies := true // bool | Include the resources this version references. (optional)
	dependencyStates := []string{"Inner_example"} // []string | Keep only the dependency versions in these states (comma-separated). Needs dependencies=true. (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CertificateVersionsAPI.RetrieveCertificateVersion(context.Background(), certificateId, versionId).Dependencies(dependencies).DependencyStates(dependencyStates).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CertificateVersionsAPI.RetrieveCertificateVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveCertificateVersion`: CertificateVersion
	fmt.Fprintf(os.Stdout, "Response from `CertificateVersionsAPI.RetrieveCertificateVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**certificateId** | **int64** | A unique value identifying the certificate. | 
**versionId** | **string** | A unique value identifying the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveCertificateVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **dependencies** | **bool** | Include the resources this version references. | 
 **dependencyStates** | **[]string** | Keep only the dependency versions in these states (comma-separated). Needs dependencies&#x3D;true. | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[**CertificateVersion**](CertificateVersion.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RevertCertificateVersion

> CertificateVersionMeta RevertCertificateVersion(ctx, certificateId, versionId).CertificateVersionRevertRequest(certificateVersionRevertRequest).Execute()

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
	certificateId := int64(789) // int64 | A unique value identifying the certificate.
	versionId := "versionId_example" // string | A unique value identifying the version.
	certificateVersionRevertRequest := *openapiclient.NewCertificateVersionRevertRequest() // CertificateVersionRevertRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CertificateVersionsAPI.RevertCertificateVersion(context.Background(), certificateId, versionId).CertificateVersionRevertRequest(certificateVersionRevertRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CertificateVersionsAPI.RevertCertificateVersion``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RevertCertificateVersion`: CertificateVersionMeta
	fmt.Fprintf(os.Stdout, "Response from `CertificateVersionsAPI.RevertCertificateVersion`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**certificateId** | **int64** | A unique value identifying the certificate. | 
**versionId** | **string** | A unique value identifying the version. | 

### Other Parameters

Other parameters are passed through a pointer to a apiRevertCertificateVersionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **certificateVersionRevertRequest** | [**CertificateVersionRevertRequest**](CertificateVersionRevertRequest.md) |  | 

### Return type

[**CertificateVersionMeta**](CertificateVersionMeta.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

