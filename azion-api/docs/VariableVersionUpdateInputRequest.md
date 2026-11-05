# VariableVersionUpdateInputRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Key** | Pointer to **string** |  | [optional] 
**Value** | Pointer to **string** |  | [optional] 
**Secret** | Pointer to **bool** |  | [optional] 
**Scope** | Pointer to [**[]ScopeItemRequest**](ScopeItemRequest.md) |  | [optional] 

## Methods

### NewVariableVersionUpdateInputRequest

`func NewVariableVersionUpdateInputRequest() *VariableVersionUpdateInputRequest`

NewVariableVersionUpdateInputRequest instantiates a new VariableVersionUpdateInputRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVariableVersionUpdateInputRequestWithDefaults

`func NewVariableVersionUpdateInputRequestWithDefaults() *VariableVersionUpdateInputRequest`

NewVariableVersionUpdateInputRequestWithDefaults instantiates a new VariableVersionUpdateInputRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKey

`func (o *VariableVersionUpdateInputRequest) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *VariableVersionUpdateInputRequest) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *VariableVersionUpdateInputRequest) SetKey(v string)`

SetKey sets Key field to given value.

### HasKey

`func (o *VariableVersionUpdateInputRequest) HasKey() bool`

HasKey returns a boolean if a field has been set.

### GetValue

`func (o *VariableVersionUpdateInputRequest) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *VariableVersionUpdateInputRequest) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *VariableVersionUpdateInputRequest) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *VariableVersionUpdateInputRequest) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetSecret

`func (o *VariableVersionUpdateInputRequest) GetSecret() bool`

GetSecret returns the Secret field if non-nil, zero value otherwise.

### GetSecretOk

`func (o *VariableVersionUpdateInputRequest) GetSecretOk() (*bool, bool)`

GetSecretOk returns a tuple with the Secret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecret

`func (o *VariableVersionUpdateInputRequest) SetSecret(v bool)`

SetSecret sets Secret field to given value.

### HasSecret

`func (o *VariableVersionUpdateInputRequest) HasSecret() bool`

HasSecret returns a boolean if a field has been set.

### GetScope

`func (o *VariableVersionUpdateInputRequest) GetScope() []ScopeItemRequest`

GetScope returns the Scope field if non-nil, zero value otherwise.

### GetScopeOk

`func (o *VariableVersionUpdateInputRequest) GetScopeOk() (*[]ScopeItemRequest, bool)`

GetScopeOk returns a tuple with the Scope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScope

`func (o *VariableVersionUpdateInputRequest) SetScope(v []ScopeItemRequest)`

SetScope sets Scope field to given value.

### HasScope

`func (o *VariableVersionUpdateInputRequest) HasScope() bool`

HasScope returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


