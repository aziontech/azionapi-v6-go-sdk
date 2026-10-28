# PatchedCacheSettingsModulesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Cache** | Pointer to [**PatchedCacheSettingsCacheModuleRequest**](PatchedCacheSettingsCacheModuleRequest.md) |  | [optional] 
**ApplicationAccelerator** | Pointer to [**PatchedCacheSettingsApplicationAcceleratorModuleRequest**](PatchedCacheSettingsApplicationAcceleratorModuleRequest.md) |  | [optional] 

## Methods

### NewPatchedCacheSettingsModulesRequest

`func NewPatchedCacheSettingsModulesRequest() *PatchedCacheSettingsModulesRequest`

NewPatchedCacheSettingsModulesRequest instantiates a new PatchedCacheSettingsModulesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedCacheSettingsModulesRequestWithDefaults

`func NewPatchedCacheSettingsModulesRequestWithDefaults() *PatchedCacheSettingsModulesRequest`

NewPatchedCacheSettingsModulesRequestWithDefaults instantiates a new PatchedCacheSettingsModulesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCache

`func (o *PatchedCacheSettingsModulesRequest) GetCache() PatchedCacheSettingsCacheModuleRequest`

GetCache returns the Cache field if non-nil, zero value otherwise.

### GetCacheOk

`func (o *PatchedCacheSettingsModulesRequest) GetCacheOk() (*PatchedCacheSettingsCacheModuleRequest, bool)`

GetCacheOk returns a tuple with the Cache field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCache

`func (o *PatchedCacheSettingsModulesRequest) SetCache(v PatchedCacheSettingsCacheModuleRequest)`

SetCache sets Cache field to given value.

### HasCache

`func (o *PatchedCacheSettingsModulesRequest) HasCache() bool`

HasCache returns a boolean if a field has been set.

### GetApplicationAccelerator

`func (o *PatchedCacheSettingsModulesRequest) GetApplicationAccelerator() PatchedCacheSettingsApplicationAcceleratorModuleRequest`

GetApplicationAccelerator returns the ApplicationAccelerator field if non-nil, zero value otherwise.

### GetApplicationAcceleratorOk

`func (o *PatchedCacheSettingsModulesRequest) GetApplicationAcceleratorOk() (*PatchedCacheSettingsApplicationAcceleratorModuleRequest, bool)`

GetApplicationAcceleratorOk returns a tuple with the ApplicationAccelerator field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApplicationAccelerator

`func (o *PatchedCacheSettingsModulesRequest) SetApplicationAccelerator(v PatchedCacheSettingsApplicationAcceleratorModuleRequest)`

SetApplicationAccelerator sets ApplicationAccelerator field to given value.

### HasApplicationAccelerator

`func (o *PatchedCacheSettingsModulesRequest) HasApplicationAccelerator() bool`

HasApplicationAccelerator returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


