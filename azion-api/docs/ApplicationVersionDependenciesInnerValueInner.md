# ApplicationVersionDependenciesInnerValueInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int64** | ID of the dependency resource. | [optional] 
**Name** | Pointer to **NullableString** | Name of the latest live version of the resource. Null when the resource is gone. | [optional] 
**Versions** | Pointer to [**[]ApplicationVersionDependenciesInnerValueInnerVersionsInner**](ApplicationVersionDependenciesInnerValueInnerVersionsInner.md) |  | [optional] 
**Dependencies** | Pointer to [**[]map[string][]ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner**](map[string][]ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner.md) | A function in the answer carries what its published version references under its own &#x60;dependencies&#x60;, in the same shape, or null while it publishes no version. No other resource carries &#x60;dependencies&#x60;, so the answer is at most two levels deep. | [optional] 

## Methods

### NewApplicationVersionDependenciesInnerValueInner

`func NewApplicationVersionDependenciesInnerValueInner() *ApplicationVersionDependenciesInnerValueInner`

NewApplicationVersionDependenciesInnerValueInner instantiates a new ApplicationVersionDependenciesInnerValueInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApplicationVersionDependenciesInnerValueInnerWithDefaults

`func NewApplicationVersionDependenciesInnerValueInnerWithDefaults() *ApplicationVersionDependenciesInnerValueInner`

NewApplicationVersionDependenciesInnerValueInnerWithDefaults instantiates a new ApplicationVersionDependenciesInnerValueInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ApplicationVersionDependenciesInnerValueInner) GetId() int64`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ApplicationVersionDependenciesInnerValueInner) GetIdOk() (*int64, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ApplicationVersionDependenciesInnerValueInner) SetId(v int64)`

SetId sets Id field to given value.

### HasId

`func (o *ApplicationVersionDependenciesInnerValueInner) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *ApplicationVersionDependenciesInnerValueInner) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ApplicationVersionDependenciesInnerValueInner) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ApplicationVersionDependenciesInnerValueInner) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ApplicationVersionDependenciesInnerValueInner) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *ApplicationVersionDependenciesInnerValueInner) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *ApplicationVersionDependenciesInnerValueInner) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetVersions

`func (o *ApplicationVersionDependenciesInnerValueInner) GetVersions() []ApplicationVersionDependenciesInnerValueInnerVersionsInner`

GetVersions returns the Versions field if non-nil, zero value otherwise.

### GetVersionsOk

`func (o *ApplicationVersionDependenciesInnerValueInner) GetVersionsOk() (*[]ApplicationVersionDependenciesInnerValueInnerVersionsInner, bool)`

GetVersionsOk returns a tuple with the Versions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersions

`func (o *ApplicationVersionDependenciesInnerValueInner) SetVersions(v []ApplicationVersionDependenciesInnerValueInnerVersionsInner)`

SetVersions sets Versions field to given value.

### HasVersions

`func (o *ApplicationVersionDependenciesInnerValueInner) HasVersions() bool`

HasVersions returns a boolean if a field has been set.

### GetDependencies

`func (o *ApplicationVersionDependenciesInnerValueInner) GetDependencies() []map[string][]ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner`

GetDependencies returns the Dependencies field if non-nil, zero value otherwise.

### GetDependenciesOk

`func (o *ApplicationVersionDependenciesInnerValueInner) GetDependenciesOk() (*[]map[string][]ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner, bool)`

GetDependenciesOk returns a tuple with the Dependencies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDependencies

`func (o *ApplicationVersionDependenciesInnerValueInner) SetDependencies(v []map[string][]ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner)`

SetDependencies sets Dependencies field to given value.

### HasDependencies

`func (o *ApplicationVersionDependenciesInnerValueInner) HasDependencies() bool`

HasDependencies returns a boolean if a field has been set.

### SetDependenciesNil

`func (o *ApplicationVersionDependenciesInnerValueInner) SetDependenciesNil(b bool)`

 SetDependenciesNil sets the value for Dependencies to be an explicit nil

### UnsetDependencies
`func (o *ApplicationVersionDependenciesInnerValueInner) UnsetDependencies()`

UnsetDependencies ensures that no value is present for Dependencies, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


