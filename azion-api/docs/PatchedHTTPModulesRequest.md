# PatchedHTTPModulesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LoadBalancer** | Pointer to [**PatchedLoadBalancerModuleRequest**](PatchedLoadBalancerModuleRequest.md) |  | [optional] 
**OriginShield** | Pointer to [**PatchedOriginShieldModuleRequest**](PatchedOriginShieldModuleRequest.md) |  | [optional] 

## Methods

### NewPatchedHTTPModulesRequest

`func NewPatchedHTTPModulesRequest() *PatchedHTTPModulesRequest`

NewPatchedHTTPModulesRequest instantiates a new PatchedHTTPModulesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedHTTPModulesRequestWithDefaults

`func NewPatchedHTTPModulesRequestWithDefaults() *PatchedHTTPModulesRequest`

NewPatchedHTTPModulesRequestWithDefaults instantiates a new PatchedHTTPModulesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLoadBalancer

`func (o *PatchedHTTPModulesRequest) GetLoadBalancer() PatchedLoadBalancerModuleRequest`

GetLoadBalancer returns the LoadBalancer field if non-nil, zero value otherwise.

### GetLoadBalancerOk

`func (o *PatchedHTTPModulesRequest) GetLoadBalancerOk() (*PatchedLoadBalancerModuleRequest, bool)`

GetLoadBalancerOk returns a tuple with the LoadBalancer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLoadBalancer

`func (o *PatchedHTTPModulesRequest) SetLoadBalancer(v PatchedLoadBalancerModuleRequest)`

SetLoadBalancer sets LoadBalancer field to given value.

### HasLoadBalancer

`func (o *PatchedHTTPModulesRequest) HasLoadBalancer() bool`

HasLoadBalancer returns a boolean if a field has been set.

### GetOriginShield

`func (o *PatchedHTTPModulesRequest) GetOriginShield() PatchedOriginShieldModuleRequest`

GetOriginShield returns the OriginShield field if non-nil, zero value otherwise.

### GetOriginShieldOk

`func (o *PatchedHTTPModulesRequest) GetOriginShieldOk() (*PatchedOriginShieldModuleRequest, bool)`

GetOriginShieldOk returns a tuple with the OriginShield field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginShield

`func (o *PatchedHTTPModulesRequest) SetOriginShield(v PatchedOriginShieldModuleRequest)`

SetOriginShield sets OriginShield field to given value.

### HasOriginShield

`func (o *PatchedHTTPModulesRequest) HasOriginShield() bool`

HasOriginShield returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


