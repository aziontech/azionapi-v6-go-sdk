# ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int64** | ID of the dependency resource. | [optional] 
**Name** | Pointer to **NullableString** | Name of the latest live version of the resource. Null when the resource is gone. | [optional] 
**Versions** | Pointer to [**[]ApplicationVersionDependenciesInnerValueInnerVersionsInner**](ApplicationVersionDependenciesInnerValueInnerVersionsInner.md) |  | [optional] 

## Methods

### NewApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner

`func NewApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner() *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner`

NewApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner instantiates a new ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInnerWithDefaults

`func NewApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInnerWithDefaults() *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner`

NewApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInnerWithDefaults instantiates a new ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner) GetId() int64`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner) GetIdOk() (*int64, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner) SetId(v int64)`

SetId sets Id field to given value.

### HasId

`func (o *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetVersions

`func (o *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner) GetVersions() []ApplicationVersionDependenciesInnerValueInnerVersionsInner`

GetVersions returns the Versions field if non-nil, zero value otherwise.

### GetVersionsOk

`func (o *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner) GetVersionsOk() (*[]ApplicationVersionDependenciesInnerValueInnerVersionsInner, bool)`

GetVersionsOk returns a tuple with the Versions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersions

`func (o *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner) SetVersions(v []ApplicationVersionDependenciesInnerValueInnerVersionsInner)`

SetVersions sets Versions field to given value.

### HasVersions

`func (o *ApplicationVersionDependenciesInnerValueInnerDependenciesInnerValueInner) HasVersions() bool`

HasVersions returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


