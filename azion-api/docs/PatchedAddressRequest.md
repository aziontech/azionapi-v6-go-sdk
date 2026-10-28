# PatchedAddressRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Active** | Pointer to **bool** | Indicates if the address is active for use | [optional] 
**Address** | Pointer to **string** | IPv4/IPv6 address or CNAME to resolve | [optional] 
**HttpPort** | Pointer to **int32** | Port number for HTTP connections | [optional] 
**HttpsPort** | Pointer to **int32** | Port number for HTTPS connections | [optional] 
**Modules** | Pointer to [**NullablePatchedAddressModulesRequest**](PatchedAddressModulesRequest.md) |  | [optional] 

## Methods

### NewPatchedAddressRequest

`func NewPatchedAddressRequest() *PatchedAddressRequest`

NewPatchedAddressRequest instantiates a new PatchedAddressRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedAddressRequestWithDefaults

`func NewPatchedAddressRequestWithDefaults() *PatchedAddressRequest`

NewPatchedAddressRequestWithDefaults instantiates a new PatchedAddressRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetActive

`func (o *PatchedAddressRequest) GetActive() bool`

GetActive returns the Active field if non-nil, zero value otherwise.

### GetActiveOk

`func (o *PatchedAddressRequest) GetActiveOk() (*bool, bool)`

GetActiveOk returns a tuple with the Active field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActive

`func (o *PatchedAddressRequest) SetActive(v bool)`

SetActive sets Active field to given value.

### HasActive

`func (o *PatchedAddressRequest) HasActive() bool`

HasActive returns a boolean if a field has been set.

### GetAddress

`func (o *PatchedAddressRequest) GetAddress() string`

GetAddress returns the Address field if non-nil, zero value otherwise.

### GetAddressOk

`func (o *PatchedAddressRequest) GetAddressOk() (*string, bool)`

GetAddressOk returns a tuple with the Address field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddress

`func (o *PatchedAddressRequest) SetAddress(v string)`

SetAddress sets Address field to given value.

### HasAddress

`func (o *PatchedAddressRequest) HasAddress() bool`

HasAddress returns a boolean if a field has been set.

### GetHttpPort

`func (o *PatchedAddressRequest) GetHttpPort() int32`

GetHttpPort returns the HttpPort field if non-nil, zero value otherwise.

### GetHttpPortOk

`func (o *PatchedAddressRequest) GetHttpPortOk() (*int32, bool)`

GetHttpPortOk returns a tuple with the HttpPort field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpPort

`func (o *PatchedAddressRequest) SetHttpPort(v int32)`

SetHttpPort sets HttpPort field to given value.

### HasHttpPort

`func (o *PatchedAddressRequest) HasHttpPort() bool`

HasHttpPort returns a boolean if a field has been set.

### GetHttpsPort

`func (o *PatchedAddressRequest) GetHttpsPort() int32`

GetHttpsPort returns the HttpsPort field if non-nil, zero value otherwise.

### GetHttpsPortOk

`func (o *PatchedAddressRequest) GetHttpsPortOk() (*int32, bool)`

GetHttpsPortOk returns a tuple with the HttpsPort field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpsPort

`func (o *PatchedAddressRequest) SetHttpsPort(v int32)`

SetHttpsPort sets HttpsPort field to given value.

### HasHttpsPort

`func (o *PatchedAddressRequest) HasHttpsPort() bool`

HasHttpsPort returns a boolean if a field has been set.

### GetModules

`func (o *PatchedAddressRequest) GetModules() PatchedAddressModulesRequest`

GetModules returns the Modules field if non-nil, zero value otherwise.

### GetModulesOk

`func (o *PatchedAddressRequest) GetModulesOk() (*PatchedAddressModulesRequest, bool)`

GetModulesOk returns a tuple with the Modules field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModules

`func (o *PatchedAddressRequest) SetModules(v PatchedAddressModulesRequest)`

SetModules sets Modules field to given value.

### HasModules

`func (o *PatchedAddressRequest) HasModules() bool`

HasModules returns a boolean if a field has been set.

### SetModulesNil

`func (o *PatchedAddressRequest) SetModulesNil(b bool)`

 SetModulesNil sets the value for Modules to be an explicit nil

### UnsetModules
`func (o *PatchedAddressRequest) UnsetModules()`

UnsetModules ensures that no value is present for Modules, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


