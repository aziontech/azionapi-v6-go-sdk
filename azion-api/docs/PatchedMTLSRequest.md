# PatchedMTLSRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **NullableBool** |  | [optional] 
**Config** | Pointer to [**NullablePatchedMTLSConfigRequest**](PatchedMTLSConfigRequest.md) |  | [optional] 

## Methods

### NewPatchedMTLSRequest

`func NewPatchedMTLSRequest() *PatchedMTLSRequest`

NewPatchedMTLSRequest instantiates a new PatchedMTLSRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedMTLSRequestWithDefaults

`func NewPatchedMTLSRequestWithDefaults() *PatchedMTLSRequest`

NewPatchedMTLSRequestWithDefaults instantiates a new PatchedMTLSRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *PatchedMTLSRequest) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *PatchedMTLSRequest) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *PatchedMTLSRequest) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *PatchedMTLSRequest) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### SetEnabledNil

`func (o *PatchedMTLSRequest) SetEnabledNil(b bool)`

 SetEnabledNil sets the value for Enabled to be an explicit nil

### UnsetEnabled
`func (o *PatchedMTLSRequest) UnsetEnabled()`

UnsetEnabled ensures that no value is present for Enabled, not even an explicit nil
### GetConfig

`func (o *PatchedMTLSRequest) GetConfig() PatchedMTLSConfigRequest`

GetConfig returns the Config field if non-nil, zero value otherwise.

### GetConfigOk

`func (o *PatchedMTLSRequest) GetConfigOk() (*PatchedMTLSConfigRequest, bool)`

GetConfigOk returns a tuple with the Config field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfig

`func (o *PatchedMTLSRequest) SetConfig(v PatchedMTLSConfigRequest)`

SetConfig sets Config field to given value.

### HasConfig

`func (o *PatchedMTLSRequest) HasConfig() bool`

HasConfig returns a boolean if a field has been set.

### SetConfigNil

`func (o *PatchedMTLSRequest) SetConfigNil(b bool)`

 SetConfigNil sets the value for Config to be an explicit nil

### UnsetConfig
`func (o *PatchedMTLSRequest) UnsetConfig()`

UnsetConfig ensures that no value is present for Config, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


