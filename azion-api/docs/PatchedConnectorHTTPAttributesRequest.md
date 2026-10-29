# PatchedConnectorHTTPAttributesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Addresses** | Pointer to [**[]PatchedAddressRequest**](PatchedAddressRequest.md) |  | [optional] 
**ConnectionOptions** | Pointer to [**PatchedHTTPConnectionOptionsRequest**](PatchedHTTPConnectionOptionsRequest.md) |  | [optional] 
**Modules** | Pointer to [**PatchedHTTPModulesRequest**](PatchedHTTPModulesRequest.md) |  | [optional] 

## Methods

### NewPatchedConnectorHTTPAttributesRequest

`func NewPatchedConnectorHTTPAttributesRequest() *PatchedConnectorHTTPAttributesRequest`

NewPatchedConnectorHTTPAttributesRequest instantiates a new PatchedConnectorHTTPAttributesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedConnectorHTTPAttributesRequestWithDefaults

`func NewPatchedConnectorHTTPAttributesRequestWithDefaults() *PatchedConnectorHTTPAttributesRequest`

NewPatchedConnectorHTTPAttributesRequestWithDefaults instantiates a new PatchedConnectorHTTPAttributesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAddresses

`func (o *PatchedConnectorHTTPAttributesRequest) GetAddresses() []PatchedAddressRequest`

GetAddresses returns the Addresses field if non-nil, zero value otherwise.

### GetAddressesOk

`func (o *PatchedConnectorHTTPAttributesRequest) GetAddressesOk() (*[]PatchedAddressRequest, bool)`

GetAddressesOk returns a tuple with the Addresses field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddresses

`func (o *PatchedConnectorHTTPAttributesRequest) SetAddresses(v []PatchedAddressRequest)`

SetAddresses sets Addresses field to given value.

### HasAddresses

`func (o *PatchedConnectorHTTPAttributesRequest) HasAddresses() bool`

HasAddresses returns a boolean if a field has been set.

### GetConnectionOptions

`func (o *PatchedConnectorHTTPAttributesRequest) GetConnectionOptions() PatchedHTTPConnectionOptionsRequest`

GetConnectionOptions returns the ConnectionOptions field if non-nil, zero value otherwise.

### GetConnectionOptionsOk

`func (o *PatchedConnectorHTTPAttributesRequest) GetConnectionOptionsOk() (*PatchedHTTPConnectionOptionsRequest, bool)`

GetConnectionOptionsOk returns a tuple with the ConnectionOptions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnectionOptions

`func (o *PatchedConnectorHTTPAttributesRequest) SetConnectionOptions(v PatchedHTTPConnectionOptionsRequest)`

SetConnectionOptions sets ConnectionOptions field to given value.

### HasConnectionOptions

`func (o *PatchedConnectorHTTPAttributesRequest) HasConnectionOptions() bool`

HasConnectionOptions returns a boolean if a field has been set.

### GetModules

`func (o *PatchedConnectorHTTPAttributesRequest) GetModules() PatchedHTTPModulesRequest`

GetModules returns the Modules field if non-nil, zero value otherwise.

### GetModulesOk

`func (o *PatchedConnectorHTTPAttributesRequest) GetModulesOk() (*PatchedHTTPModulesRequest, bool)`

GetModulesOk returns a tuple with the Modules field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModules

`func (o *PatchedConnectorHTTPAttributesRequest) SetModules(v PatchedHTTPModulesRequest)`

SetModules sets Modules field to given value.

### HasModules

`func (o *PatchedConnectorHTTPAttributesRequest) HasModules() bool`

HasModules returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


