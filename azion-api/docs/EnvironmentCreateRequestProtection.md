# EnvironmentCreateRequestProtection

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AzionAuthentication** | Pointer to [**EnvironmentCreateRequestProtectionAzionAuthentication**](EnvironmentCreateRequestProtectionAzionAuthentication.md) |  | [optional] 
**PasswordProtection** | Pointer to [**EnvironmentCreateRequestProtectionPasswordProtection**](EnvironmentCreateRequestProtectionPasswordProtection.md) |  | [optional] 
**IpAllowlist** | Pointer to [**EnvironmentCreateRequestProtectionIpAllowlist**](EnvironmentCreateRequestProtectionIpAllowlist.md) |  | [optional] 
**SsoEnforcement** | Pointer to [**EnvironmentCreateRequestProtectionSsoEnforcement**](EnvironmentCreateRequestProtectionSsoEnforcement.md) |  | [optional] 

## Methods

### NewEnvironmentCreateRequestProtection

`func NewEnvironmentCreateRequestProtection() *EnvironmentCreateRequestProtection`

NewEnvironmentCreateRequestProtection instantiates a new EnvironmentCreateRequestProtection object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEnvironmentCreateRequestProtectionWithDefaults

`func NewEnvironmentCreateRequestProtectionWithDefaults() *EnvironmentCreateRequestProtection`

NewEnvironmentCreateRequestProtectionWithDefaults instantiates a new EnvironmentCreateRequestProtection object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAzionAuthentication

`func (o *EnvironmentCreateRequestProtection) GetAzionAuthentication() EnvironmentCreateRequestProtectionAzionAuthentication`

GetAzionAuthentication returns the AzionAuthentication field if non-nil, zero value otherwise.

### GetAzionAuthenticationOk

`func (o *EnvironmentCreateRequestProtection) GetAzionAuthenticationOk() (*EnvironmentCreateRequestProtectionAzionAuthentication, bool)`

GetAzionAuthenticationOk returns a tuple with the AzionAuthentication field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAzionAuthentication

`func (o *EnvironmentCreateRequestProtection) SetAzionAuthentication(v EnvironmentCreateRequestProtectionAzionAuthentication)`

SetAzionAuthentication sets AzionAuthentication field to given value.

### HasAzionAuthentication

`func (o *EnvironmentCreateRequestProtection) HasAzionAuthentication() bool`

HasAzionAuthentication returns a boolean if a field has been set.

### GetPasswordProtection

`func (o *EnvironmentCreateRequestProtection) GetPasswordProtection() EnvironmentCreateRequestProtectionPasswordProtection`

GetPasswordProtection returns the PasswordProtection field if non-nil, zero value otherwise.

### GetPasswordProtectionOk

`func (o *EnvironmentCreateRequestProtection) GetPasswordProtectionOk() (*EnvironmentCreateRequestProtectionPasswordProtection, bool)`

GetPasswordProtectionOk returns a tuple with the PasswordProtection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPasswordProtection

`func (o *EnvironmentCreateRequestProtection) SetPasswordProtection(v EnvironmentCreateRequestProtectionPasswordProtection)`

SetPasswordProtection sets PasswordProtection field to given value.

### HasPasswordProtection

`func (o *EnvironmentCreateRequestProtection) HasPasswordProtection() bool`

HasPasswordProtection returns a boolean if a field has been set.

### GetIpAllowlist

`func (o *EnvironmentCreateRequestProtection) GetIpAllowlist() EnvironmentCreateRequestProtectionIpAllowlist`

GetIpAllowlist returns the IpAllowlist field if non-nil, zero value otherwise.

### GetIpAllowlistOk

`func (o *EnvironmentCreateRequestProtection) GetIpAllowlistOk() (*EnvironmentCreateRequestProtectionIpAllowlist, bool)`

GetIpAllowlistOk returns a tuple with the IpAllowlist field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIpAllowlist

`func (o *EnvironmentCreateRequestProtection) SetIpAllowlist(v EnvironmentCreateRequestProtectionIpAllowlist)`

SetIpAllowlist sets IpAllowlist field to given value.

### HasIpAllowlist

`func (o *EnvironmentCreateRequestProtection) HasIpAllowlist() bool`

HasIpAllowlist returns a boolean if a field has been set.

### GetSsoEnforcement

`func (o *EnvironmentCreateRequestProtection) GetSsoEnforcement() EnvironmentCreateRequestProtectionSsoEnforcement`

GetSsoEnforcement returns the SsoEnforcement field if non-nil, zero value otherwise.

### GetSsoEnforcementOk

`func (o *EnvironmentCreateRequestProtection) GetSsoEnforcementOk() (*EnvironmentCreateRequestProtectionSsoEnforcement, bool)`

GetSsoEnforcementOk returns a tuple with the SsoEnforcement field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSsoEnforcement

`func (o *EnvironmentCreateRequestProtection) SetSsoEnforcement(v EnvironmentCreateRequestProtectionSsoEnforcement)`

SetSsoEnforcement sets SsoEnforcement field to given value.

### HasSsoEnforcement

`func (o *EnvironmentCreateRequestProtection) HasSsoEnforcement() bool`

HasSsoEnforcement returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


