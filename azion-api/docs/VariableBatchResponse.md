# VariableBatchResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Created** | Pointer to [**[]Variable**](Variable.md) |  | [optional] 
**Updated** | Pointer to [**[]Variable**](Variable.md) |  | [optional] 
**Deleted** | Pointer to **[]string** |  | [optional] 

## Methods

### NewVariableBatchResponse

`func NewVariableBatchResponse() *VariableBatchResponse`

NewVariableBatchResponse instantiates a new VariableBatchResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVariableBatchResponseWithDefaults

`func NewVariableBatchResponseWithDefaults() *VariableBatchResponse`

NewVariableBatchResponseWithDefaults instantiates a new VariableBatchResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCreated

`func (o *VariableBatchResponse) GetCreated() []Variable`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *VariableBatchResponse) GetCreatedOk() (*[]Variable, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *VariableBatchResponse) SetCreated(v []Variable)`

SetCreated sets Created field to given value.

### HasCreated

`func (o *VariableBatchResponse) HasCreated() bool`

HasCreated returns a boolean if a field has been set.

### GetUpdated

`func (o *VariableBatchResponse) GetUpdated() []Variable`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *VariableBatchResponse) GetUpdatedOk() (*[]Variable, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *VariableBatchResponse) SetUpdated(v []Variable)`

SetUpdated sets Updated field to given value.

### HasUpdated

`func (o *VariableBatchResponse) HasUpdated() bool`

HasUpdated returns a boolean if a field has been set.

### GetDeleted

`func (o *VariableBatchResponse) GetDeleted() []string`

GetDeleted returns the Deleted field if non-nil, zero value otherwise.

### GetDeletedOk

`func (o *VariableBatchResponse) GetDeletedOk() (*[]string, bool)`

GetDeletedOk returns a tuple with the Deleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeleted

`func (o *VariableBatchResponse) SetDeleted(v []string)`

SetDeleted sets Deleted field to given value.

### HasDeleted

`func (o *VariableBatchResponse) HasDeleted() bool`

HasDeleted returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


