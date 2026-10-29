# EnvironmentProtectionSsoEnforcement

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | **bool** |  | 
**IdpId** | **NullableString** |  | 
**AllowedDomains** | **[]string** |  | 

## Methods

### NewEnvironmentProtectionSsoEnforcement

`func NewEnvironmentProtectionSsoEnforcement(enabled bool, idpId NullableString, allowedDomains []string, ) *EnvironmentProtectionSsoEnforcement`

NewEnvironmentProtectionSsoEnforcement instantiates a new EnvironmentProtectionSsoEnforcement object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEnvironmentProtectionSsoEnforcementWithDefaults

`func NewEnvironmentProtectionSsoEnforcementWithDefaults() *EnvironmentProtectionSsoEnforcement`

NewEnvironmentProtectionSsoEnforcementWithDefaults instantiates a new EnvironmentProtectionSsoEnforcement object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *EnvironmentProtectionSsoEnforcement) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *EnvironmentProtectionSsoEnforcement) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *EnvironmentProtectionSsoEnforcement) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.


### GetIdpId

`func (o *EnvironmentProtectionSsoEnforcement) GetIdpId() string`

GetIdpId returns the IdpId field if non-nil, zero value otherwise.

### GetIdpIdOk

`func (o *EnvironmentProtectionSsoEnforcement) GetIdpIdOk() (*string, bool)`

GetIdpIdOk returns a tuple with the IdpId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIdpId

`func (o *EnvironmentProtectionSsoEnforcement) SetIdpId(v string)`

SetIdpId sets IdpId field to given value.


### SetIdpIdNil

`func (o *EnvironmentProtectionSsoEnforcement) SetIdpIdNil(b bool)`

 SetIdpIdNil sets the value for IdpId to be an explicit nil

### UnsetIdpId
`func (o *EnvironmentProtectionSsoEnforcement) UnsetIdpId()`

UnsetIdpId ensures that no value is present for IdpId, not even an explicit nil
### GetAllowedDomains

`func (o *EnvironmentProtectionSsoEnforcement) GetAllowedDomains() []string`

GetAllowedDomains returns the AllowedDomains field if non-nil, zero value otherwise.

### GetAllowedDomainsOk

`func (o *EnvironmentProtectionSsoEnforcement) GetAllowedDomainsOk() (*[]string, bool)`

GetAllowedDomainsOk returns a tuple with the AllowedDomains field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllowedDomains

`func (o *EnvironmentProtectionSsoEnforcement) SetAllowedDomains(v []string)`

SetAllowedDomains sets AllowedDomains field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


