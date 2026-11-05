# DependencyEntry

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** | * &#x60;connector&#x60; - connector * &#x60;network_list&#x60; - network_list | 
**Id** | Pointer to **NullableInt64** |  | [optional] 

## Methods

### NewDependencyEntry

`func NewDependencyEntry(type_ string, ) *DependencyEntry`

NewDependencyEntry instantiates a new DependencyEntry object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDependencyEntryWithDefaults

`func NewDependencyEntryWithDefaults() *DependencyEntry`

NewDependencyEntryWithDefaults instantiates a new DependencyEntry object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *DependencyEntry) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *DependencyEntry) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *DependencyEntry) SetType(v string)`

SetType sets Type field to given value.


### GetId

`func (o *DependencyEntry) GetId() int64`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *DependencyEntry) GetIdOk() (*int64, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *DependencyEntry) SetId(v int64)`

SetId sets Id field to given value.

### HasId

`func (o *DependencyEntry) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *DependencyEntry) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *DependencyEntry) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


