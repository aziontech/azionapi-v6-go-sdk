# PatchedCacheSettingsCacheModuleRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Behavior** | Pointer to **string** | * &#x60;honor&#x60; - Honor Origin Cache Settings * &#x60;override&#x60; - Override Cache Settings | [optional] 
**MaxAge** | Pointer to **int32** | To use a value lower than 60s, the Application Acceleration module must be enabled on the Application. | [optional] 
**StaleCache** | Pointer to [**PatchedStateCacheModuleRequest**](PatchedStateCacheModuleRequest.md) |  | [optional] 
**LargeFileCache** | Pointer to [**PatchedLargeFileCacheModuleRequest**](PatchedLargeFileCacheModuleRequest.md) |  | [optional] 
**TieredCache** | Pointer to [**NullablePatchedCacheSettingsTieredCacheModuleRequest**](PatchedCacheSettingsTieredCacheModuleRequest.md) |  | [optional] 

## Methods

### NewPatchedCacheSettingsCacheModuleRequest

`func NewPatchedCacheSettingsCacheModuleRequest() *PatchedCacheSettingsCacheModuleRequest`

NewPatchedCacheSettingsCacheModuleRequest instantiates a new PatchedCacheSettingsCacheModuleRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedCacheSettingsCacheModuleRequestWithDefaults

`func NewPatchedCacheSettingsCacheModuleRequestWithDefaults() *PatchedCacheSettingsCacheModuleRequest`

NewPatchedCacheSettingsCacheModuleRequestWithDefaults instantiates a new PatchedCacheSettingsCacheModuleRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBehavior

`func (o *PatchedCacheSettingsCacheModuleRequest) GetBehavior() string`

GetBehavior returns the Behavior field if non-nil, zero value otherwise.

### GetBehaviorOk

`func (o *PatchedCacheSettingsCacheModuleRequest) GetBehaviorOk() (*string, bool)`

GetBehaviorOk returns a tuple with the Behavior field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBehavior

`func (o *PatchedCacheSettingsCacheModuleRequest) SetBehavior(v string)`

SetBehavior sets Behavior field to given value.

### HasBehavior

`func (o *PatchedCacheSettingsCacheModuleRequest) HasBehavior() bool`

HasBehavior returns a boolean if a field has been set.

### GetMaxAge

`func (o *PatchedCacheSettingsCacheModuleRequest) GetMaxAge() int32`

GetMaxAge returns the MaxAge field if non-nil, zero value otherwise.

### GetMaxAgeOk

`func (o *PatchedCacheSettingsCacheModuleRequest) GetMaxAgeOk() (*int32, bool)`

GetMaxAgeOk returns a tuple with the MaxAge field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxAge

`func (o *PatchedCacheSettingsCacheModuleRequest) SetMaxAge(v int32)`

SetMaxAge sets MaxAge field to given value.

### HasMaxAge

`func (o *PatchedCacheSettingsCacheModuleRequest) HasMaxAge() bool`

HasMaxAge returns a boolean if a field has been set.

### GetStaleCache

`func (o *PatchedCacheSettingsCacheModuleRequest) GetStaleCache() PatchedStateCacheModuleRequest`

GetStaleCache returns the StaleCache field if non-nil, zero value otherwise.

### GetStaleCacheOk

`func (o *PatchedCacheSettingsCacheModuleRequest) GetStaleCacheOk() (*PatchedStateCacheModuleRequest, bool)`

GetStaleCacheOk returns a tuple with the StaleCache field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStaleCache

`func (o *PatchedCacheSettingsCacheModuleRequest) SetStaleCache(v PatchedStateCacheModuleRequest)`

SetStaleCache sets StaleCache field to given value.

### HasStaleCache

`func (o *PatchedCacheSettingsCacheModuleRequest) HasStaleCache() bool`

HasStaleCache returns a boolean if a field has been set.

### GetLargeFileCache

`func (o *PatchedCacheSettingsCacheModuleRequest) GetLargeFileCache() PatchedLargeFileCacheModuleRequest`

GetLargeFileCache returns the LargeFileCache field if non-nil, zero value otherwise.

### GetLargeFileCacheOk

`func (o *PatchedCacheSettingsCacheModuleRequest) GetLargeFileCacheOk() (*PatchedLargeFileCacheModuleRequest, bool)`

GetLargeFileCacheOk returns a tuple with the LargeFileCache field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLargeFileCache

`func (o *PatchedCacheSettingsCacheModuleRequest) SetLargeFileCache(v PatchedLargeFileCacheModuleRequest)`

SetLargeFileCache sets LargeFileCache field to given value.

### HasLargeFileCache

`func (o *PatchedCacheSettingsCacheModuleRequest) HasLargeFileCache() bool`

HasLargeFileCache returns a boolean if a field has been set.

### GetTieredCache

`func (o *PatchedCacheSettingsCacheModuleRequest) GetTieredCache() PatchedCacheSettingsTieredCacheModuleRequest`

GetTieredCache returns the TieredCache field if non-nil, zero value otherwise.

### GetTieredCacheOk

`func (o *PatchedCacheSettingsCacheModuleRequest) GetTieredCacheOk() (*PatchedCacheSettingsTieredCacheModuleRequest, bool)`

GetTieredCacheOk returns a tuple with the TieredCache field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTieredCache

`func (o *PatchedCacheSettingsCacheModuleRequest) SetTieredCache(v PatchedCacheSettingsTieredCacheModuleRequest)`

SetTieredCache sets TieredCache field to given value.

### HasTieredCache

`func (o *PatchedCacheSettingsCacheModuleRequest) HasTieredCache() bool`

HasTieredCache returns a boolean if a field has been set.

### SetTieredCacheNil

`func (o *PatchedCacheSettingsCacheModuleRequest) SetTieredCacheNil(b bool)`

 SetTieredCacheNil sets the value for TieredCache to be an explicit nil

### UnsetTieredCache
`func (o *PatchedCacheSettingsCacheModuleRequest) UnsetTieredCache()`

UnsetTieredCache ensures that no value is present for TieredCache, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


