# PatchedDeploymentRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **NullableString** |  | [optional] 
**BindingPolicy** | Pointer to **string** | * &#x60;STRICT&#x60; - STRICT * &#x60;FLEXIBLE&#x60; - FLEXIBLE | [optional] 
**DeploymentPolicy** | Pointer to **string** | * &#x60;single_version&#x60; - single_version * &#x60;versioned_urls&#x60; - versioned_urls | [optional] 
**StrategyDefaults** | Pointer to [**DeploymentStrategyDefaults**](DeploymentStrategyDefaults.md) |  | [optional] 

## Methods

### NewPatchedDeploymentRequest

`func NewPatchedDeploymentRequest() *PatchedDeploymentRequest`

NewPatchedDeploymentRequest instantiates a new PatchedDeploymentRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedDeploymentRequestWithDefaults

`func NewPatchedDeploymentRequestWithDefaults() *PatchedDeploymentRequest`

NewPatchedDeploymentRequestWithDefaults instantiates a new PatchedDeploymentRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *PatchedDeploymentRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *PatchedDeploymentRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *PatchedDeploymentRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *PatchedDeploymentRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *PatchedDeploymentRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *PatchedDeploymentRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *PatchedDeploymentRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *PatchedDeploymentRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *PatchedDeploymentRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *PatchedDeploymentRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetBindingPolicy

`func (o *PatchedDeploymentRequest) GetBindingPolicy() string`

GetBindingPolicy returns the BindingPolicy field if non-nil, zero value otherwise.

### GetBindingPolicyOk

`func (o *PatchedDeploymentRequest) GetBindingPolicyOk() (*string, bool)`

GetBindingPolicyOk returns a tuple with the BindingPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBindingPolicy

`func (o *PatchedDeploymentRequest) SetBindingPolicy(v string)`

SetBindingPolicy sets BindingPolicy field to given value.

### HasBindingPolicy

`func (o *PatchedDeploymentRequest) HasBindingPolicy() bool`

HasBindingPolicy returns a boolean if a field has been set.

### GetDeploymentPolicy

`func (o *PatchedDeploymentRequest) GetDeploymentPolicy() string`

GetDeploymentPolicy returns the DeploymentPolicy field if non-nil, zero value otherwise.

### GetDeploymentPolicyOk

`func (o *PatchedDeploymentRequest) GetDeploymentPolicyOk() (*string, bool)`

GetDeploymentPolicyOk returns a tuple with the DeploymentPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentPolicy

`func (o *PatchedDeploymentRequest) SetDeploymentPolicy(v string)`

SetDeploymentPolicy sets DeploymentPolicy field to given value.

### HasDeploymentPolicy

`func (o *PatchedDeploymentRequest) HasDeploymentPolicy() bool`

HasDeploymentPolicy returns a boolean if a field has been set.

### GetStrategyDefaults

`func (o *PatchedDeploymentRequest) GetStrategyDefaults() DeploymentStrategyDefaults`

GetStrategyDefaults returns the StrategyDefaults field if non-nil, zero value otherwise.

### GetStrategyDefaultsOk

`func (o *PatchedDeploymentRequest) GetStrategyDefaultsOk() (*DeploymentStrategyDefaults, bool)`

GetStrategyDefaultsOk returns a tuple with the StrategyDefaults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStrategyDefaults

`func (o *PatchedDeploymentRequest) SetStrategyDefaults(v DeploymentStrategyDefaults)`

SetStrategyDefaults sets StrategyDefaults field to given value.

### HasStrategyDefaults

`func (o *PatchedDeploymentRequest) HasStrategyDefaults() bool`

HasStrategyDefaults returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


