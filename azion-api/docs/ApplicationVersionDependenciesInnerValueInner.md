# ApplicationVersionDependenciesInnerValueInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int64** | ID of the dependency resource. | [optional] 
**Name** | Pointer to **NullableString** | Name of the latest live version of the resource. Null when the resource is gone. | [optional] 
**Versions** | Pointer to [**[]ApplicationVersionDependenciesInnerValueInnerVersionsInner**](ApplicationVersionDependenciesInnerValueInnerVersionsInner.md) |  | [optional] 

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


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


