# VariableVersionCreateInputRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Key** | **string** |  | 
**Value** | **string** |  | 
**Secret** | Pointer to **bool** |  | [optional] 
**Scope** | Pointer to [**[]ScopeItemRequest**](ScopeItemRequest.md) |  | [optional] 

## Methods

### NewVariableVersionCreateInputRequest

`func NewVariableVersionCreateInputRequest(key string, value string, ) *VariableVersionCreateInputRequest`

NewVariableVersionCreateInputRequest instantiates a new VariableVersionCreateInputRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVariableVersionCreateInputRequestWithDefaults

`func NewVariableVersionCreateInputRequestWithDefaults() *VariableVersionCreateInputRequest`

NewVariableVersionCreateInputRequestWithDefaults instantiates a new VariableVersionCreateInputRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKey

`func (o *VariableVersionCreateInputRequest) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *VariableVersionCreateInputRequest) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *VariableVersionCreateInputRequest) SetKey(v string)`

SetKey sets Key field to given value.


### GetValue

`func (o *VariableVersionCreateInputRequest) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *VariableVersionCreateInputRequest) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *VariableVersionCreateInputRequest) SetValue(v string)`

SetValue sets Value field to given value.


### GetSecret

`func (o *VariableVersionCreateInputRequest) GetSecret() bool`

GetSecret returns the Secret field if non-nil, zero value otherwise.

### GetSecretOk

`func (o *VariableVersionCreateInputRequest) GetSecretOk() (*bool, bool)`

GetSecretOk returns a tuple with the Secret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecret

`func (o *VariableVersionCreateInputRequest) SetSecret(v bool)`

SetSecret sets Secret field to given value.

### HasSecret

`func (o *VariableVersionCreateInputRequest) HasSecret() bool`

HasSecret returns a boolean if a field has been set.

### GetScope

`func (o *VariableVersionCreateInputRequest) GetScope() []ScopeItemRequest`

GetScope returns the Scope field if non-nil, zero value otherwise.

### GetScopeOk

`func (o *VariableVersionCreateInputRequest) GetScopeOk() (*[]ScopeItemRequest, bool)`

GetScopeOk returns a tuple with the Scope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScope

`func (o *VariableVersionCreateInputRequest) SetScope(v []ScopeItemRequest)`

SetScope sets Scope field to given value.

### HasScope

`func (o *VariableVersionCreateInputRequest) HasScope() bool`

HasScope returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


