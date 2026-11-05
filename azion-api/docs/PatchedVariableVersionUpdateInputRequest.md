# PatchedVariableVersionUpdateInputRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Key** | Pointer to **string** |  | [optional] 
**Value** | Pointer to **string** |  | [optional] 
**Secret** | Pointer to **bool** |  | [optional] 
**Scope** | Pointer to [**[]PatchedScopeItemRequest**](PatchedScopeItemRequest.md) |  | [optional] 

## Methods

### NewPatchedVariableVersionUpdateInputRequest

`func NewPatchedVariableVersionUpdateInputRequest() *PatchedVariableVersionUpdateInputRequest`

NewPatchedVariableVersionUpdateInputRequest instantiates a new PatchedVariableVersionUpdateInputRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedVariableVersionUpdateInputRequestWithDefaults

`func NewPatchedVariableVersionUpdateInputRequestWithDefaults() *PatchedVariableVersionUpdateInputRequest`

NewPatchedVariableVersionUpdateInputRequestWithDefaults instantiates a new PatchedVariableVersionUpdateInputRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKey

`func (o *PatchedVariableVersionUpdateInputRequest) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *PatchedVariableVersionUpdateInputRequest) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *PatchedVariableVersionUpdateInputRequest) SetKey(v string)`

SetKey sets Key field to given value.

### HasKey

`func (o *PatchedVariableVersionUpdateInputRequest) HasKey() bool`

HasKey returns a boolean if a field has been set.

### GetValue

`func (o *PatchedVariableVersionUpdateInputRequest) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *PatchedVariableVersionUpdateInputRequest) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *PatchedVariableVersionUpdateInputRequest) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *PatchedVariableVersionUpdateInputRequest) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetSecret

`func (o *PatchedVariableVersionUpdateInputRequest) GetSecret() bool`

GetSecret returns the Secret field if non-nil, zero value otherwise.

### GetSecretOk

`func (o *PatchedVariableVersionUpdateInputRequest) GetSecretOk() (*bool, bool)`

GetSecretOk returns a tuple with the Secret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecret

`func (o *PatchedVariableVersionUpdateInputRequest) SetSecret(v bool)`

SetSecret sets Secret field to given value.

### HasSecret

`func (o *PatchedVariableVersionUpdateInputRequest) HasSecret() bool`

HasSecret returns a boolean if a field has been set.

### GetScope

`func (o *PatchedVariableVersionUpdateInputRequest) GetScope() []PatchedScopeItemRequest`

GetScope returns the Scope field if non-nil, zero value otherwise.

### GetScopeOk

`func (o *PatchedVariableVersionUpdateInputRequest) GetScopeOk() (*[]PatchedScopeItemRequest, bool)`

GetScopeOk returns a tuple with the Scope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScope

`func (o *PatchedVariableVersionUpdateInputRequest) SetScope(v []PatchedScopeItemRequest)`

SetScope sets Scope field to given value.

### HasScope

`func (o *PatchedVariableVersionUpdateInputRequest) HasScope() bool`

HasScope returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


