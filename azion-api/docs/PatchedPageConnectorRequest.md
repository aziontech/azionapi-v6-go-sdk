# PatchedPageConnectorRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** |  | 
**Attributes** | Pointer to [**PatchedPageConnectorAttributesRequest**](PatchedPageConnectorAttributesRequest.md) |  | [optional] 

## Methods

### NewPatchedPageConnectorRequest

`func NewPatchedPageConnectorRequest(type_ string, ) *PatchedPageConnectorRequest`

NewPatchedPageConnectorRequest instantiates a new PatchedPageConnectorRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedPageConnectorRequestWithDefaults

`func NewPatchedPageConnectorRequestWithDefaults() *PatchedPageConnectorRequest`

NewPatchedPageConnectorRequestWithDefaults instantiates a new PatchedPageConnectorRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *PatchedPageConnectorRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *PatchedPageConnectorRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *PatchedPageConnectorRequest) SetType(v string)`

SetType sets Type field to given value.


### GetAttributes

`func (o *PatchedPageConnectorRequest) GetAttributes() PatchedPageConnectorAttributesRequest`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *PatchedPageConnectorRequest) GetAttributesOk() (*PatchedPageConnectorAttributesRequest, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *PatchedPageConnectorRequest) SetAttributes(v PatchedPageConnectorAttributesRequest)`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *PatchedPageConnectorRequest) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


