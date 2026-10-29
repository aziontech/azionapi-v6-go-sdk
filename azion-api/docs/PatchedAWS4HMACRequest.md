# PatchedAWS4HMACRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | Pointer to **string** | * &#x60;aws4_hmac_sha256&#x60; - AWS for HMAC - SHA256 | [optional] 
**Attributes** | Pointer to [**PatchedAWS4HMACAttributesRequest**](PatchedAWS4HMACAttributesRequest.md) |  | [optional] 

## Methods

### NewPatchedAWS4HMACRequest

`func NewPatchedAWS4HMACRequest() *PatchedAWS4HMACRequest`

NewPatchedAWS4HMACRequest instantiates a new PatchedAWS4HMACRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedAWS4HMACRequestWithDefaults

`func NewPatchedAWS4HMACRequestWithDefaults() *PatchedAWS4HMACRequest`

NewPatchedAWS4HMACRequestWithDefaults instantiates a new PatchedAWS4HMACRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *PatchedAWS4HMACRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *PatchedAWS4HMACRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *PatchedAWS4HMACRequest) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *PatchedAWS4HMACRequest) HasType() bool`

HasType returns a boolean if a field has been set.

### GetAttributes

`func (o *PatchedAWS4HMACRequest) GetAttributes() PatchedAWS4HMACAttributesRequest`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *PatchedAWS4HMACRequest) GetAttributesOk() (*PatchedAWS4HMACAttributesRequest, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *PatchedAWS4HMACRequest) SetAttributes(v PatchedAWS4HMACAttributesRequest)`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *PatchedAWS4HMACRequest) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


