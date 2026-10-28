# \DeploymentsReleaseRoutingAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ActivateRelease**](DeploymentsReleaseRoutingAPI.md#ActivateRelease) | **Post** /deployments/{deployment_id}/releases/{release_id}/activate | Activate a release



## ActivateRelease

> ReleaseAsyncResponse ActivateRelease(ctx, deploymentId, releaseId).ActivateReleaseRequest(activateReleaseRequest).Execute()

Activate a release



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
	releaseId := "releaseId_example" // string | A unique value identifying the release.
	activateReleaseRequest := *openapiclient.NewActivateReleaseRequest() // ActivateReleaseRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DeploymentsReleaseRoutingAPI.ActivateRelease(context.Background(), deploymentId, releaseId).ActivateReleaseRequest(activateReleaseRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DeploymentsReleaseRoutingAPI.ActivateRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ActivateRelease`: ReleaseAsyncResponse
	fmt.Fprintf(os.Stdout, "Response from `DeploymentsReleaseRoutingAPI.ActivateRelease`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**deploymentId** | **string** | A unique value identifying the deployment. | 
**releaseId** | **string** | A unique value identifying the release. | 

### Other Parameters

Other parameters are passed through a pointer to a apiActivateReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **activateReleaseRequest** | [**ActivateReleaseRequest**](ActivateReleaseRequest.md) |  | 

### Return type

[**ReleaseAsyncResponse**](ReleaseAsyncResponse.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

