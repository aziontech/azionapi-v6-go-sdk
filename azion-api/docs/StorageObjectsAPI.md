# \StorageObjectsAPI

All URIs are relative to *https://api.azion.com/v6*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CopyObject**](StorageObjectsAPI.md#CopyObject) | **Post** /workspace/storage/buckets/{bucket_name}/objects/{object_key}/copy/{new_object_key} | Copy object to new key
[**CreateObject**](StorageObjectsAPI.md#CreateObject) | **Post** /workspace/storage/buckets/{bucket_name}/objects/{object_key} | Create new object key.
[**DeleteObject**](StorageObjectsAPI.md#DeleteObject) | **Delete** /workspace/storage/buckets/{bucket_name}/objects/{object_key} | Delete object key
[**ListObjects**](StorageObjectsAPI.md#ListObjects) | **Get** /workspace/storage/buckets/{bucket_name}/objects | List objects from bucket
[**RetrieveObject**](StorageObjectsAPI.md#RetrieveObject) | **Get** /workspace/storage/buckets/{bucket_name}/objects/{object_key} | Download object
[**UpdateObject**](StorageObjectsAPI.md#UpdateObject) | **Put** /workspace/storage/buckets/{bucket_name}/objects/{object_key} | Update the object key.



## CopyObject

> SuccessObjectOperation CopyObject(ctx, bucketName, newObjectKey, objectKey).Body(body).Execute()

Copy object to new key



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
	bucketName := "bucketName_example" // string | The name of the bucket
	newObjectKey := "newObjectKey_example" // string | The key/path of the destination object within the bucket
	objectKey := "objectKey_example" // string | The key/path of the source object within the bucket
	body := map[string]interface{}{ ... } // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageObjectsAPI.CopyObject(context.Background(), bucketName, newObjectKey, objectKey).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageObjectsAPI.CopyObject``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CopyObject`: SuccessObjectOperation
	fmt.Fprintf(os.Stdout, "Response from `StorageObjectsAPI.CopyObject`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**bucketName** | **string** | The name of the bucket | 
**newObjectKey** | **string** | The key/path of the destination object within the bucket | 
**objectKey** | **string** | The key/path of the source object within the bucket | 

### Other Parameters

Other parameters are passed through a pointer to a apiCopyObjectRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **body** | **map[string]interface{}** |  | 

### Return type

[**SuccessObjectOperation**](SuccessObjectOperation.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateObject

> SuccessObjectOperation CreateObject(ctx, bucketName, objectKey).ContentType(contentType).Body(body).Execute()

Create new object key.



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
	bucketName := "bucketName_example" // string | The name of the bucket
	objectKey := "objectKey_example" // string | The key/path of the object within the bucket
	contentType := "contentType_example" // string | The MIME type of the object being uploaded (optional)
	body := os.NewFile(1234, "some_file") // *os.File |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageObjectsAPI.CreateObject(context.Background(), bucketName, objectKey).ContentType(contentType).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageObjectsAPI.CreateObject``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateObject`: SuccessObjectOperation
	fmt.Fprintf(os.Stdout, "Response from `StorageObjectsAPI.CreateObject`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**bucketName** | **string** | The name of the bucket | 
**objectKey** | **string** | The key/path of the object within the bucket | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateObjectRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **contentType** | **string** | The MIME type of the object being uploaded | 
 **body** | ***os.File** |  | 

### Return type

[**SuccessObjectOperation**](SuccessObjectOperation.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/octet-stream
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteObject

> DeleteResponse DeleteObject(ctx, bucketName, objectKey).Execute()

Delete object key



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
	bucketName := "bucketName_example" // string | The name of the bucket
	objectKey := "objectKey_example" // string | The key/path of the object within the bucket

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageObjectsAPI.DeleteObject(context.Background(), bucketName, objectKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageObjectsAPI.DeleteObject``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteObject`: DeleteResponse
	fmt.Fprintf(os.Stdout, "Response from `StorageObjectsAPI.DeleteObject`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**bucketName** | **string** | The name of the bucket | 
**objectKey** | **string** | The key/path of the object within the bucket | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteObjectRequest struct via the builder pattern


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


## ListObjects

> ResponseBucketObject ListObjects(ctx, bucketName).AllLevels(allLevels).ContinuationToken(continuationToken).Fields(fields).MaxObjectCount(maxObjectCount).Prefix(prefix).Execute()

List objects from bucket



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
	bucketName := "bucketName_example" // string | The name of the bucket
	allLevels := true // bool | If true, lists objects recursively. If false, lists only the first level using Delimiter='/' (default: true). (optional)
	continuationToken := "continuationToken_example" // string | A continuation token for the next page of records. (optional)
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)
	maxObjectCount := int64(789) // int64 | Number of results to be returned on the page. Limited to 1000 objects. (optional)
	prefix := "prefix_example" // string | Filter objects by key prefix. If empty, lists from the bucket root (default: empty). (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageObjectsAPI.ListObjects(context.Background(), bucketName).AllLevels(allLevels).ContinuationToken(continuationToken).Fields(fields).MaxObjectCount(maxObjectCount).Prefix(prefix).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageObjectsAPI.ListObjects``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListObjects`: ResponseBucketObject
	fmt.Fprintf(os.Stdout, "Response from `StorageObjectsAPI.ListObjects`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**bucketName** | **string** | The name of the bucket | 

### Other Parameters

Other parameters are passed through a pointer to a apiListObjectsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **allLevels** | **bool** | If true, lists objects recursively. If false, lists only the first level using Delimiter&#x3D;&#39;/&#39; (default: true). | 
 **continuationToken** | **string** | A continuation token for the next page of records. | 
 **fields** | **string** | Comma-separated list of field names to include in the response. | 
 **maxObjectCount** | **int64** | Number of results to be returned on the page. Limited to 1000 objects. | 
 **prefix** | **string** | Filter objects by key prefix. If empty, lists from the bucket root (default: empty). | 

### Return type

[**ResponseBucketObject**](ResponseBucketObject.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RetrieveObject

> *os.File RetrieveObject(ctx, bucketName, objectKey).Fields(fields).Execute()

Download object



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
	bucketName := "bucketName_example" // string | The name of the bucket
	objectKey := "objectKey_example" // string | The key/path of the object within the bucket
	fields := "fields_example" // string | Comma-separated list of field names to include in the response. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageObjectsAPI.RetrieveObject(context.Background(), bucketName, objectKey).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageObjectsAPI.RetrieveObject``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RetrieveObject`: *os.File
	fmt.Fprintf(os.Stdout, "Response from `StorageObjectsAPI.RetrieveObject`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**bucketName** | **string** | The name of the bucket | 
**objectKey** | **string** | The key/path of the object within the bucket | 

### Other Parameters

Other parameters are passed through a pointer to a apiRetrieveObjectRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **fields** | **string** | Comma-separated list of field names to include in the response. | 

### Return type

[***os.File**](*os.File.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateObject

> SuccessObjectOperation UpdateObject(ctx, bucketName, objectKey).ContentType(contentType).Body(body).Execute()

Update the object key.



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
	bucketName := "bucketName_example" // string | The name of the bucket
	objectKey := "objectKey_example" // string | The key/path of the object within the bucket
	contentType := "contentType_example" // string | The MIME type of the object being uploaded (optional)
	body := os.NewFile(1234, "some_file") // *os.File |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StorageObjectsAPI.UpdateObject(context.Background(), bucketName, objectKey).ContentType(contentType).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StorageObjectsAPI.UpdateObject``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateObject`: SuccessObjectOperation
	fmt.Fprintf(os.Stdout, "Response from `StorageObjectsAPI.UpdateObject`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**bucketName** | **string** | The name of the bucket | 
**objectKey** | **string** | The key/path of the object within the bucket | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateObjectRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **contentType** | **string** | The MIME type of the object being uploaded | 
 **body** | ***os.File** |  | 

### Return type

[**SuccessObjectOperation**](SuccessObjectOperation.md)

### Authorization

[TokenAuth](../README.md#TokenAuth), [BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/octet-stream
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

