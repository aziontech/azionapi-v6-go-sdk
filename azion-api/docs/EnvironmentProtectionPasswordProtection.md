# EnvironmentProtectionPasswordProtection

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | **bool** |  | 
**SecretId** | **NullableString** |  | 

## Methods

### NewEnvironmentProtectionPasswordProtection

`func NewEnvironmentProtectionPasswordProtection(enabled bool, secretId NullableString, ) *EnvironmentProtectionPasswordProtection`

NewEnvironmentProtectionPasswordProtection instantiates a new EnvironmentProtectionPasswordProtection object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEnvironmentProtectionPasswordProtectionWithDefaults

`func NewEnvironmentProtectionPasswordProtectionWithDefaults() *EnvironmentProtectionPasswordProtection`

NewEnvironmentProtectionPasswordProtectionWithDefaults instantiates a new EnvironmentProtectionPasswordProtection object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *EnvironmentProtectionPasswordProtection) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *EnvironmentProtectionPasswordProtection) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *EnvironmentProtectionPasswordProtection) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.


### GetSecretId

`func (o *EnvironmentProtectionPasswordProtection) GetSecretId() string`

GetSecretId returns the SecretId field if non-nil, zero value otherwise.

### GetSecretIdOk

`func (o *EnvironmentProtectionPasswordProtection) GetSecretIdOk() (*string, bool)`

GetSecretIdOk returns a tuple with the SecretId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecretId

`func (o *EnvironmentProtectionPasswordProtection) SetSecretId(v string)`

SetSecretId sets SecretId field to given value.


### SetSecretIdNil

`func (o *EnvironmentProtectionPasswordProtection) SetSecretIdNil(b bool)`

 SetSecretIdNil sets the value for SecretId to be an explicit nil

### UnsetSecretId
`func (o *EnvironmentProtectionPasswordProtection) UnsetSecretId()`

UnsetSecretId ensures that no value is present for SecretId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


