# EnvironmentCreateRequestProtectionSsoEnforcement

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | **bool** |  | 
**IdpId** | **NullableString** |  | 
**AllowedDomains** | **[]string** |  | 

## Methods

### NewEnvironmentCreateRequestProtectionSsoEnforcement

`func NewEnvironmentCreateRequestProtectionSsoEnforcement(enabled bool, idpId NullableString, allowedDomains []string, ) *EnvironmentCreateRequestProtectionSsoEnforcement`

NewEnvironmentCreateRequestProtectionSsoEnforcement instantiates a new EnvironmentCreateRequestProtectionSsoEnforcement object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEnvironmentCreateRequestProtectionSsoEnforcementWithDefaults

`func NewEnvironmentCreateRequestProtectionSsoEnforcementWithDefaults() *EnvironmentCreateRequestProtectionSsoEnforcement`

NewEnvironmentCreateRequestProtectionSsoEnforcementWithDefaults instantiates a new EnvironmentCreateRequestProtectionSsoEnforcement object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *EnvironmentCreateRequestProtectionSsoEnforcement) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *EnvironmentCreateRequestProtectionSsoEnforcement) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *EnvironmentCreateRequestProtectionSsoEnforcement) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.


### GetIdpId

`func (o *EnvironmentCreateRequestProtectionSsoEnforcement) GetIdpId() string`

GetIdpId returns the IdpId field if non-nil, zero value otherwise.

### GetIdpIdOk

`func (o *EnvironmentCreateRequestProtectionSsoEnforcement) GetIdpIdOk() (*string, bool)`

GetIdpIdOk returns a tuple with the IdpId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIdpId

`func (o *EnvironmentCreateRequestProtectionSsoEnforcement) SetIdpId(v string)`

SetIdpId sets IdpId field to given value.


### SetIdpIdNil

`func (o *EnvironmentCreateRequestProtectionSsoEnforcement) SetIdpIdNil(b bool)`

 SetIdpIdNil sets the value for IdpId to be an explicit nil

### UnsetIdpId
`func (o *EnvironmentCreateRequestProtectionSsoEnforcement) UnsetIdpId()`

UnsetIdpId ensures that no value is present for IdpId, not even an explicit nil
### GetAllowedDomains

`func (o *EnvironmentCreateRequestProtectionSsoEnforcement) GetAllowedDomains() []string`

GetAllowedDomains returns the AllowedDomains field if non-nil, zero value otherwise.

### GetAllowedDomainsOk

`func (o *EnvironmentCreateRequestProtectionSsoEnforcement) GetAllowedDomainsOk() (*[]string, bool)`

GetAllowedDomainsOk returns a tuple with the AllowedDomains field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAllowedDomains

`func (o *EnvironmentCreateRequestProtectionSsoEnforcement) SetAllowedDomains(v []string)`

SetAllowedDomains sets AllowedDomains field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


