# PatchedHMACRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** |  | [optional] 
**Config** | Pointer to [**NullablePatchedAWS4HMACRequest**](PatchedAWS4HMACRequest.md) |  | [optional] 

## Methods

### NewPatchedHMACRequest

`func NewPatchedHMACRequest() *PatchedHMACRequest`

NewPatchedHMACRequest instantiates a new PatchedHMACRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedHMACRequestWithDefaults

`func NewPatchedHMACRequestWithDefaults() *PatchedHMACRequest`

NewPatchedHMACRequestWithDefaults instantiates a new PatchedHMACRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *PatchedHMACRequest) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *PatchedHMACRequest) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *PatchedHMACRequest) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *PatchedHMACRequest) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetConfig

`func (o *PatchedHMACRequest) GetConfig() PatchedAWS4HMACRequest`

GetConfig returns the Config field if non-nil, zero value otherwise.

### GetConfigOk

`func (o *PatchedHMACRequest) GetConfigOk() (*PatchedAWS4HMACRequest, bool)`

GetConfigOk returns a tuple with the Config field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfig

`func (o *PatchedHMACRequest) SetConfig(v PatchedAWS4HMACRequest)`

SetConfig sets Config field to given value.

### HasConfig

`func (o *PatchedHMACRequest) HasConfig() bool`

HasConfig returns a boolean if a field has been set.

### SetConfigNil

`func (o *PatchedHMACRequest) SetConfigNil(b bool)`

 SetConfigNil sets the value for Config to be an explicit nil

### UnsetConfig
`func (o *PatchedHMACRequest) UnsetConfig()`

UnsetConfig ensures that no value is present for Config, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


