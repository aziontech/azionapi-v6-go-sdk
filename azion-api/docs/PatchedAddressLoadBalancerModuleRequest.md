# PatchedAddressLoadBalancerModuleRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ServerRole** | Pointer to **string** | Role of the address in load balancing  * &#x60;primary&#x60; - Primary * &#x60;backup&#x60; - Backup | [optional] 
**Weight** | Pointer to **int32** | Weight used in load balancing strategy | [optional] 

## Methods

### NewPatchedAddressLoadBalancerModuleRequest

`func NewPatchedAddressLoadBalancerModuleRequest() *PatchedAddressLoadBalancerModuleRequest`

NewPatchedAddressLoadBalancerModuleRequest instantiates a new PatchedAddressLoadBalancerModuleRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedAddressLoadBalancerModuleRequestWithDefaults

`func NewPatchedAddressLoadBalancerModuleRequestWithDefaults() *PatchedAddressLoadBalancerModuleRequest`

NewPatchedAddressLoadBalancerModuleRequestWithDefaults instantiates a new PatchedAddressLoadBalancerModuleRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetServerRole

`func (o *PatchedAddressLoadBalancerModuleRequest) GetServerRole() string`

GetServerRole returns the ServerRole field if non-nil, zero value otherwise.

### GetServerRoleOk

`func (o *PatchedAddressLoadBalancerModuleRequest) GetServerRoleOk() (*string, bool)`

GetServerRoleOk returns a tuple with the ServerRole field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServerRole

`func (o *PatchedAddressLoadBalancerModuleRequest) SetServerRole(v string)`

SetServerRole sets ServerRole field to given value.

### HasServerRole

`func (o *PatchedAddressLoadBalancerModuleRequest) HasServerRole() bool`

HasServerRole returns a boolean if a field has been set.

### GetWeight

`func (o *PatchedAddressLoadBalancerModuleRequest) GetWeight() int32`

GetWeight returns the Weight field if non-nil, zero value otherwise.

### GetWeightOk

`func (o *PatchedAddressLoadBalancerModuleRequest) GetWeightOk() (*int32, bool)`

GetWeightOk returns a tuple with the Weight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWeight

`func (o *PatchedAddressLoadBalancerModuleRequest) SetWeight(v int32)`

SetWeight sets Weight field to given value.

### HasWeight

`func (o *PatchedAddressLoadBalancerModuleRequest) HasWeight() bool`

HasWeight returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


