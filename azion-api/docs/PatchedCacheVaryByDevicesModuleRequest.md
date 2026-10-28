# PatchedCacheVaryByDevicesModuleRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Behavior** | Pointer to **string** | * &#x60;ignore&#x60; - ignore * &#x60;allowlist&#x60; - allowlist | [optional] 
**DeviceGroup** | Pointer to **[]int64** |  | [optional] 

## Methods

### NewPatchedCacheVaryByDevicesModuleRequest

`func NewPatchedCacheVaryByDevicesModuleRequest() *PatchedCacheVaryByDevicesModuleRequest`

NewPatchedCacheVaryByDevicesModuleRequest instantiates a new PatchedCacheVaryByDevicesModuleRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedCacheVaryByDevicesModuleRequestWithDefaults

`func NewPatchedCacheVaryByDevicesModuleRequestWithDefaults() *PatchedCacheVaryByDevicesModuleRequest`

NewPatchedCacheVaryByDevicesModuleRequestWithDefaults instantiates a new PatchedCacheVaryByDevicesModuleRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBehavior

`func (o *PatchedCacheVaryByDevicesModuleRequest) GetBehavior() string`

GetBehavior returns the Behavior field if non-nil, zero value otherwise.

### GetBehaviorOk

`func (o *PatchedCacheVaryByDevicesModuleRequest) GetBehaviorOk() (*string, bool)`

GetBehaviorOk returns a tuple with the Behavior field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBehavior

`func (o *PatchedCacheVaryByDevicesModuleRequest) SetBehavior(v string)`

SetBehavior sets Behavior field to given value.

### HasBehavior

`func (o *PatchedCacheVaryByDevicesModuleRequest) HasBehavior() bool`

HasBehavior returns a boolean if a field has been set.

### GetDeviceGroup

`func (o *PatchedCacheVaryByDevicesModuleRequest) GetDeviceGroup() []int64`

GetDeviceGroup returns the DeviceGroup field if non-nil, zero value otherwise.

### GetDeviceGroupOk

`func (o *PatchedCacheVaryByDevicesModuleRequest) GetDeviceGroupOk() (*[]int64, bool)`

GetDeviceGroupOk returns a tuple with the DeviceGroup field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeviceGroup

`func (o *PatchedCacheVaryByDevicesModuleRequest) SetDeviceGroup(v []int64)`

SetDeviceGroup sets DeviceGroup field to given value.

### HasDeviceGroup

`func (o *PatchedCacheVaryByDevicesModuleRequest) HasDeviceGroup() bool`

HasDeviceGroup returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


