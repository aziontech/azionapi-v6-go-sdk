# VariableBatchUpdateItemRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Key** | Pointer to **string** |  | [optional] 
**Value** | Pointer to **string** |  | [optional] 
**Secret** | Pointer to **bool** |  | [optional] 
**Uuid** | **string** |  | 

## Methods

### NewVariableBatchUpdateItemRequest

`func NewVariableBatchUpdateItemRequest(uuid string, ) *VariableBatchUpdateItemRequest`

NewVariableBatchUpdateItemRequest instantiates a new VariableBatchUpdateItemRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVariableBatchUpdateItemRequestWithDefaults

`func NewVariableBatchUpdateItemRequestWithDefaults() *VariableBatchUpdateItemRequest`

NewVariableBatchUpdateItemRequestWithDefaults instantiates a new VariableBatchUpdateItemRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKey

`func (o *VariableBatchUpdateItemRequest) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *VariableBatchUpdateItemRequest) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *VariableBatchUpdateItemRequest) SetKey(v string)`

SetKey sets Key field to given value.

### HasKey

`func (o *VariableBatchUpdateItemRequest) HasKey() bool`

HasKey returns a boolean if a field has been set.

### GetValue

`func (o *VariableBatchUpdateItemRequest) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *VariableBatchUpdateItemRequest) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *VariableBatchUpdateItemRequest) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *VariableBatchUpdateItemRequest) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetSecret

`func (o *VariableBatchUpdateItemRequest) GetSecret() bool`

GetSecret returns the Secret field if non-nil, zero value otherwise.

### GetSecretOk

`func (o *VariableBatchUpdateItemRequest) GetSecretOk() (*bool, bool)`

GetSecretOk returns a tuple with the Secret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecret

`func (o *VariableBatchUpdateItemRequest) SetSecret(v bool)`

SetSecret sets Secret field to given value.

### HasSecret

`func (o *VariableBatchUpdateItemRequest) HasSecret() bool`

HasSecret returns a boolean if a field has been set.

### GetUuid

`func (o *VariableBatchUpdateItemRequest) GetUuid() string`

GetUuid returns the Uuid field if non-nil, zero value otherwise.

### GetUuidOk

`func (o *VariableBatchUpdateItemRequest) GetUuidOk() (*string, bool)`

GetUuidOk returns a tuple with the Uuid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUuid

`func (o *VariableBatchUpdateItemRequest) SetUuid(v string)`

SetUuid sets Uuid field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


