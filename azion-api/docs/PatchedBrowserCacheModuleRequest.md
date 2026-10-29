# PatchedBrowserCacheModuleRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Behavior** | Pointer to **string** | * &#x60;override&#x60; - override * &#x60;honor&#x60; - honor * &#x60;no-cache&#x60; - no-cache | [optional] 
**MaxAge** | Pointer to **int32** |  | [optional] 

## Methods

### NewPatchedBrowserCacheModuleRequest

`func NewPatchedBrowserCacheModuleRequest() *PatchedBrowserCacheModuleRequest`

NewPatchedBrowserCacheModuleRequest instantiates a new PatchedBrowserCacheModuleRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedBrowserCacheModuleRequestWithDefaults

`func NewPatchedBrowserCacheModuleRequestWithDefaults() *PatchedBrowserCacheModuleRequest`

NewPatchedBrowserCacheModuleRequestWithDefaults instantiates a new PatchedBrowserCacheModuleRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBehavior

`func (o *PatchedBrowserCacheModuleRequest) GetBehavior() string`

GetBehavior returns the Behavior field if non-nil, zero value otherwise.

### GetBehaviorOk

`func (o *PatchedBrowserCacheModuleRequest) GetBehaviorOk() (*string, bool)`

GetBehaviorOk returns a tuple with the Behavior field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBehavior

`func (o *PatchedBrowserCacheModuleRequest) SetBehavior(v string)`

SetBehavior sets Behavior field to given value.

### HasBehavior

`func (o *PatchedBrowserCacheModuleRequest) HasBehavior() bool`

HasBehavior returns a boolean if a field has been set.

### GetMaxAge

`func (o *PatchedBrowserCacheModuleRequest) GetMaxAge() int32`

GetMaxAge returns the MaxAge field if non-nil, zero value otherwise.

### GetMaxAgeOk

`func (o *PatchedBrowserCacheModuleRequest) GetMaxAgeOk() (*int32, bool)`

GetMaxAgeOk returns a tuple with the MaxAge field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxAge

`func (o *PatchedBrowserCacheModuleRequest) SetMaxAge(v int32)`

SetMaxAge sets MaxAge field to given value.

### HasMaxAge

`func (o *PatchedBrowserCacheModuleRequest) HasMaxAge() bool`

HasMaxAge returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


