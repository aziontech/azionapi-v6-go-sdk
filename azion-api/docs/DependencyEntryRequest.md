# DependencyEntryRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** | * &#x60;connector&#x60; - connector * &#x60;network_list&#x60; - network_list | 
**Id** | Pointer to **NullableInt64** |  | [optional] 

## Methods

### NewDependencyEntryRequest

`func NewDependencyEntryRequest(type_ string, ) *DependencyEntryRequest`

NewDependencyEntryRequest instantiates a new DependencyEntryRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDependencyEntryRequestWithDefaults

`func NewDependencyEntryRequestWithDefaults() *DependencyEntryRequest`

NewDependencyEntryRequestWithDefaults instantiates a new DependencyEntryRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *DependencyEntryRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *DependencyEntryRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *DependencyEntryRequest) SetType(v string)`

SetType sets Type field to given value.


### GetId

`func (o *DependencyEntryRequest) GetId() int64`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *DependencyEntryRequest) GetIdOk() (*int64, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *DependencyEntryRequest) SetId(v int64)`

SetId sets Id field to given value.

### HasId

`func (o *DependencyEntryRequest) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *DependencyEntryRequest) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *DependencyEntryRequest) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


