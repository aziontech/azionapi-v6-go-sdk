# DeploymentCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**BindingPolicy** | **string** | * &#x60;STRICT&#x60; - STRICT * &#x60;FLEXIBLE&#x60; - FLEXIBLE | 
**DeploymentPolicy** | Pointer to **string** | * &#x60;single_version&#x60; - single_version * &#x60;versioned_urls&#x60; - versioned_urls | [optional] 
**StrategyDefaults** | Pointer to [**DeploymentStrategyDefaults**](DeploymentStrategyDefaults.md) |  | [optional] 

## Methods

### NewDeploymentCreateRequest

`func NewDeploymentCreateRequest(name string, bindingPolicy string, ) *DeploymentCreateRequest`

NewDeploymentCreateRequest instantiates a new DeploymentCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeploymentCreateRequestWithDefaults

`func NewDeploymentCreateRequestWithDefaults() *DeploymentCreateRequest`

NewDeploymentCreateRequestWithDefaults instantiates a new DeploymentCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *DeploymentCreateRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *DeploymentCreateRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *DeploymentCreateRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *DeploymentCreateRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *DeploymentCreateRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *DeploymentCreateRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *DeploymentCreateRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *DeploymentCreateRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *DeploymentCreateRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetBindingPolicy

`func (o *DeploymentCreateRequest) GetBindingPolicy() string`

GetBindingPolicy returns the BindingPolicy field if non-nil, zero value otherwise.

### GetBindingPolicyOk

`func (o *DeploymentCreateRequest) GetBindingPolicyOk() (*string, bool)`

GetBindingPolicyOk returns a tuple with the BindingPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBindingPolicy

`func (o *DeploymentCreateRequest) SetBindingPolicy(v string)`

SetBindingPolicy sets BindingPolicy field to given value.


### GetDeploymentPolicy

`func (o *DeploymentCreateRequest) GetDeploymentPolicy() string`

GetDeploymentPolicy returns the DeploymentPolicy field if non-nil, zero value otherwise.

### GetDeploymentPolicyOk

`func (o *DeploymentCreateRequest) GetDeploymentPolicyOk() (*string, bool)`

GetDeploymentPolicyOk returns a tuple with the DeploymentPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentPolicy

`func (o *DeploymentCreateRequest) SetDeploymentPolicy(v string)`

SetDeploymentPolicy sets DeploymentPolicy field to given value.

### HasDeploymentPolicy

`func (o *DeploymentCreateRequest) HasDeploymentPolicy() bool`

HasDeploymentPolicy returns a boolean if a field has been set.

### GetStrategyDefaults

`func (o *DeploymentCreateRequest) GetStrategyDefaults() DeploymentStrategyDefaults`

GetStrategyDefaults returns the StrategyDefaults field if non-nil, zero value otherwise.

### GetStrategyDefaultsOk

`func (o *DeploymentCreateRequest) GetStrategyDefaultsOk() (*DeploymentStrategyDefaults, bool)`

GetStrategyDefaultsOk returns a tuple with the StrategyDefaults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStrategyDefaults

`func (o *DeploymentCreateRequest) SetStrategyDefaults(v DeploymentStrategyDefaults)`

SetStrategyDefaults sets StrategyDefaults field to given value.

### HasStrategyDefaults

`func (o *DeploymentCreateRequest) HasStrategyDefaults() bool`

HasStrategyDefaults returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


