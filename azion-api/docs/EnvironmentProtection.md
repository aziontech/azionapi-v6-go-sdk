# EnvironmentProtection

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AzionAuthentication** | [**EnvironmentProtectionAzionAuthentication**](EnvironmentProtectionAzionAuthentication.md) |  | 
**PasswordProtection** | [**EnvironmentProtectionPasswordProtection**](EnvironmentProtectionPasswordProtection.md) |  | 
**IpAllowlist** | [**EnvironmentProtectionIpAllowlist**](EnvironmentProtectionIpAllowlist.md) |  | 
**SsoEnforcement** | [**EnvironmentProtectionSsoEnforcement**](EnvironmentProtectionSsoEnforcement.md) |  | 

## Methods

### NewEnvironmentProtection

`func NewEnvironmentProtection(azionAuthentication EnvironmentProtectionAzionAuthentication, passwordProtection EnvironmentProtectionPasswordProtection, ipAllowlist EnvironmentProtectionIpAllowlist, ssoEnforcement EnvironmentProtectionSsoEnforcement, ) *EnvironmentProtection`

NewEnvironmentProtection instantiates a new EnvironmentProtection object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEnvironmentProtectionWithDefaults

`func NewEnvironmentProtectionWithDefaults() *EnvironmentProtection`

NewEnvironmentProtectionWithDefaults instantiates a new EnvironmentProtection object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAzionAuthentication

`func (o *EnvironmentProtection) GetAzionAuthentication() EnvironmentProtectionAzionAuthentication`

GetAzionAuthentication returns the AzionAuthentication field if non-nil, zero value otherwise.

### GetAzionAuthenticationOk

`func (o *EnvironmentProtection) GetAzionAuthenticationOk() (*EnvironmentProtectionAzionAuthentication, bool)`

GetAzionAuthenticationOk returns a tuple with the AzionAuthentication field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAzionAuthentication

`func (o *EnvironmentProtection) SetAzionAuthentication(v EnvironmentProtectionAzionAuthentication)`

SetAzionAuthentication sets AzionAuthentication field to given value.


### GetPasswordProtection

`func (o *EnvironmentProtection) GetPasswordProtection() EnvironmentProtectionPasswordProtection`

GetPasswordProtection returns the PasswordProtection field if non-nil, zero value otherwise.

### GetPasswordProtectionOk

`func (o *EnvironmentProtection) GetPasswordProtectionOk() (*EnvironmentProtectionPasswordProtection, bool)`

GetPasswordProtectionOk returns a tuple with the PasswordProtection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPasswordProtection

`func (o *EnvironmentProtection) SetPasswordProtection(v EnvironmentProtectionPasswordProtection)`

SetPasswordProtection sets PasswordProtection field to given value.


### GetIpAllowlist

`func (o *EnvironmentProtection) GetIpAllowlist() EnvironmentProtectionIpAllowlist`

GetIpAllowlist returns the IpAllowlist field if non-nil, zero value otherwise.

### GetIpAllowlistOk

`func (o *EnvironmentProtection) GetIpAllowlistOk() (*EnvironmentProtectionIpAllowlist, bool)`

GetIpAllowlistOk returns a tuple with the IpAllowlist field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIpAllowlist

`func (o *EnvironmentProtection) SetIpAllowlist(v EnvironmentProtectionIpAllowlist)`

SetIpAllowlist sets IpAllowlist field to given value.


### GetSsoEnforcement

`func (o *EnvironmentProtection) GetSsoEnforcement() EnvironmentProtectionSsoEnforcement`

GetSsoEnforcement returns the SsoEnforcement field if non-nil, zero value otherwise.

### GetSsoEnforcementOk

`func (o *EnvironmentProtection) GetSsoEnforcementOk() (*EnvironmentProtectionSsoEnforcement, bool)`

GetSsoEnforcementOk returns a tuple with the SsoEnforcement field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSsoEnforcement

`func (o *EnvironmentProtection) SetSsoEnforcement(v EnvironmentProtectionSsoEnforcement)`

SetSsoEnforcement sets SsoEnforcement field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


