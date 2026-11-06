# PatchedConnectorStorageBaseRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Type** | Pointer to **string** |  | [optional] 
**Attributes** | Pointer to [**PatchedConnectorStorageAttributesRequest**](PatchedConnectorStorageAttributesRequest.md) |  | [optional] 

## Methods

### NewPatchedConnectorStorageBaseRequest

`func NewPatchedConnectorStorageBaseRequest() *PatchedConnectorStorageBaseRequest`

NewPatchedConnectorStorageBaseRequest instantiates a new PatchedConnectorStorageBaseRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedConnectorStorageBaseRequestWithDefaults

`func NewPatchedConnectorStorageBaseRequestWithDefaults() *PatchedConnectorStorageBaseRequest`

NewPatchedConnectorStorageBaseRequestWithDefaults instantiates a new PatchedConnectorStorageBaseRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *PatchedConnectorStorageBaseRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *PatchedConnectorStorageBaseRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *PatchedConnectorStorageBaseRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *PatchedConnectorStorageBaseRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetType

`func (o *PatchedConnectorStorageBaseRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *PatchedConnectorStorageBaseRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *PatchedConnectorStorageBaseRequest) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *PatchedConnectorStorageBaseRequest) HasType() bool`

HasType returns a boolean if a field has been set.

### GetAttributes

`func (o *PatchedConnectorStorageBaseRequest) GetAttributes() PatchedConnectorStorageAttributesRequest`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *PatchedConnectorStorageBaseRequest) GetAttributesOk() (*PatchedConnectorStorageAttributesRequest, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *PatchedConnectorStorageBaseRequest) SetAttributes(v PatchedConnectorStorageAttributesRequest)`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *PatchedConnectorStorageBaseRequest) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


