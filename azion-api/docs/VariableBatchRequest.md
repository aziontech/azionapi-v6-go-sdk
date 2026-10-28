# VariableBatchRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Create** | Pointer to [**[]VariableVersionCreateInputRequest**](VariableVersionCreateInputRequest.md) |  | [optional] 
**Update** | Pointer to [**[]VariableBatchUpdateItemRequest**](VariableBatchUpdateItemRequest.md) |  | [optional] 
**Delete** | Pointer to **[]string** |  | [optional] 

## Methods

### NewVariableBatchRequest

`func NewVariableBatchRequest() *VariableBatchRequest`

NewVariableBatchRequest instantiates a new VariableBatchRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVariableBatchRequestWithDefaults

`func NewVariableBatchRequestWithDefaults() *VariableBatchRequest`

NewVariableBatchRequestWithDefaults instantiates a new VariableBatchRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCreate

`func (o *VariableBatchRequest) GetCreate() []VariableVersionCreateInputRequest`

GetCreate returns the Create field if non-nil, zero value otherwise.

### GetCreateOk

`func (o *VariableBatchRequest) GetCreateOk() (*[]VariableVersionCreateInputRequest, bool)`

GetCreateOk returns a tuple with the Create field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreate

`func (o *VariableBatchRequest) SetCreate(v []VariableVersionCreateInputRequest)`

SetCreate sets Create field to given value.

### HasCreate

`func (o *VariableBatchRequest) HasCreate() bool`

HasCreate returns a boolean if a field has been set.

### GetUpdate

`func (o *VariableBatchRequest) GetUpdate() []VariableBatchUpdateItemRequest`

GetUpdate returns the Update field if non-nil, zero value otherwise.

### GetUpdateOk

`func (o *VariableBatchRequest) GetUpdateOk() (*[]VariableBatchUpdateItemRequest, bool)`

GetUpdateOk returns a tuple with the Update field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdate

`func (o *VariableBatchRequest) SetUpdate(v []VariableBatchUpdateItemRequest)`

SetUpdate sets Update field to given value.

### HasUpdate

`func (o *VariableBatchRequest) HasUpdate() bool`

HasUpdate returns a boolean if a field has been set.

### GetDelete

`func (o *VariableBatchRequest) GetDelete() []string`

GetDelete returns the Delete field if non-nil, zero value otherwise.

### GetDeleteOk

`func (o *VariableBatchRequest) GetDeleteOk() (*[]string, bool)`

GetDeleteOk returns a tuple with the Delete field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDelete

`func (o *VariableBatchRequest) SetDelete(v []string)`

SetDelete sets Delete field to given value.

### HasDelete

`func (o *VariableBatchRequest) HasDelete() bool`

HasDelete returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


