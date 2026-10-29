# PatchedLoadBalancerModuleRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** |  | [optional] 
**Config** | Pointer to [**NullablePatchedLoadBalancerModuleConfigRequest**](PatchedLoadBalancerModuleConfigRequest.md) |  | [optional] 

## Methods

### NewPatchedLoadBalancerModuleRequest

`func NewPatchedLoadBalancerModuleRequest() *PatchedLoadBalancerModuleRequest`

NewPatchedLoadBalancerModuleRequest instantiates a new PatchedLoadBalancerModuleRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedLoadBalancerModuleRequestWithDefaults

`func NewPatchedLoadBalancerModuleRequestWithDefaults() *PatchedLoadBalancerModuleRequest`

NewPatchedLoadBalancerModuleRequestWithDefaults instantiates a new PatchedLoadBalancerModuleRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *PatchedLoadBalancerModuleRequest) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *PatchedLoadBalancerModuleRequest) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *PatchedLoadBalancerModuleRequest) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *PatchedLoadBalancerModuleRequest) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetConfig

`func (o *PatchedLoadBalancerModuleRequest) GetConfig() PatchedLoadBalancerModuleConfigRequest`

GetConfig returns the Config field if non-nil, zero value otherwise.

### GetConfigOk

`func (o *PatchedLoadBalancerModuleRequest) GetConfigOk() (*PatchedLoadBalancerModuleConfigRequest, bool)`

GetConfigOk returns a tuple with the Config field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfig

`func (o *PatchedLoadBalancerModuleRequest) SetConfig(v PatchedLoadBalancerModuleConfigRequest)`

SetConfig sets Config field to given value.

### HasConfig

`func (o *PatchedLoadBalancerModuleRequest) HasConfig() bool`

HasConfig returns a boolean if a field has been set.

### SetConfigNil

`func (o *PatchedLoadBalancerModuleRequest) SetConfigNil(b bool)`

 SetConfigNil sets the value for Config to be an explicit nil

### UnsetConfig
`func (o *PatchedLoadBalancerModuleRequest) UnsetConfig()`

UnsetConfig ensures that no value is present for Config, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


