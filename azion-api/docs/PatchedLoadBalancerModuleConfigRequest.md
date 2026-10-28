# PatchedLoadBalancerModuleConfigRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Method** | Pointer to **string** | Load balancing method to use (e.g., round-robin, least_conn).  * &#x60;round_robin&#x60; - Round Robin * &#x60;least_conn&#x60; - Least Connections * &#x60;ip_hash&#x60; - IP Hash | [optional] 
**MaxRetries** | Pointer to **int32** | Maximum number of retry attempts on connection failure. | [optional] 
**ConnectionTimeout** | Pointer to **int32** | Maximum time (in seconds) to wait for a connection to be established. | [optional] 
**ReadWriteTimeout** | Pointer to **int32** | Maximum time (in seconds) to wait for data read/write after connection. | [optional] 

## Methods

### NewPatchedLoadBalancerModuleConfigRequest

`func NewPatchedLoadBalancerModuleConfigRequest() *PatchedLoadBalancerModuleConfigRequest`

NewPatchedLoadBalancerModuleConfigRequest instantiates a new PatchedLoadBalancerModuleConfigRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedLoadBalancerModuleConfigRequestWithDefaults

`func NewPatchedLoadBalancerModuleConfigRequestWithDefaults() *PatchedLoadBalancerModuleConfigRequest`

NewPatchedLoadBalancerModuleConfigRequestWithDefaults instantiates a new PatchedLoadBalancerModuleConfigRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMethod

`func (o *PatchedLoadBalancerModuleConfigRequest) GetMethod() string`

GetMethod returns the Method field if non-nil, zero value otherwise.

### GetMethodOk

`func (o *PatchedLoadBalancerModuleConfigRequest) GetMethodOk() (*string, bool)`

GetMethodOk returns a tuple with the Method field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMethod

`func (o *PatchedLoadBalancerModuleConfigRequest) SetMethod(v string)`

SetMethod sets Method field to given value.

### HasMethod

`func (o *PatchedLoadBalancerModuleConfigRequest) HasMethod() bool`

HasMethod returns a boolean if a field has been set.

### GetMaxRetries

`func (o *PatchedLoadBalancerModuleConfigRequest) GetMaxRetries() int32`

GetMaxRetries returns the MaxRetries field if non-nil, zero value otherwise.

### GetMaxRetriesOk

`func (o *PatchedLoadBalancerModuleConfigRequest) GetMaxRetriesOk() (*int32, bool)`

GetMaxRetriesOk returns a tuple with the MaxRetries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxRetries

`func (o *PatchedLoadBalancerModuleConfigRequest) SetMaxRetries(v int32)`

SetMaxRetries sets MaxRetries field to given value.

### HasMaxRetries

`func (o *PatchedLoadBalancerModuleConfigRequest) HasMaxRetries() bool`

HasMaxRetries returns a boolean if a field has been set.

### GetConnectionTimeout

`func (o *PatchedLoadBalancerModuleConfigRequest) GetConnectionTimeout() int32`

GetConnectionTimeout returns the ConnectionTimeout field if non-nil, zero value otherwise.

### GetConnectionTimeoutOk

`func (o *PatchedLoadBalancerModuleConfigRequest) GetConnectionTimeoutOk() (*int32, bool)`

GetConnectionTimeoutOk returns a tuple with the ConnectionTimeout field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnectionTimeout

`func (o *PatchedLoadBalancerModuleConfigRequest) SetConnectionTimeout(v int32)`

SetConnectionTimeout sets ConnectionTimeout field to given value.

### HasConnectionTimeout

`func (o *PatchedLoadBalancerModuleConfigRequest) HasConnectionTimeout() bool`

HasConnectionTimeout returns a boolean if a field has been set.

### GetReadWriteTimeout

`func (o *PatchedLoadBalancerModuleConfigRequest) GetReadWriteTimeout() int32`

GetReadWriteTimeout returns the ReadWriteTimeout field if non-nil, zero value otherwise.

### GetReadWriteTimeoutOk

`func (o *PatchedLoadBalancerModuleConfigRequest) GetReadWriteTimeoutOk() (*int32, bool)`

GetReadWriteTimeoutOk returns a tuple with the ReadWriteTimeout field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadWriteTimeout

`func (o *PatchedLoadBalancerModuleConfigRequest) SetReadWriteTimeout(v int32)`

SetReadWriteTimeout sets ReadWriteTimeout field to given value.

### HasReadWriteTimeout

`func (o *PatchedLoadBalancerModuleConfigRequest) HasReadWriteTimeout() bool`

HasReadWriteTimeout returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


