# PatchedApplicationModulesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Cache** | Pointer to [**PatchedCacheModuleRequest**](PatchedCacheModuleRequest.md) |  | [optional] 
**Functions** | Pointer to [**PatchedFunctionModuleRequest**](PatchedFunctionModuleRequest.md) |  | [optional] 
**ApplicationAccelerator** | Pointer to [**PatchedApplicationAcceleratorModuleRequest**](PatchedApplicationAcceleratorModuleRequest.md) |  | [optional] 
**ImageProcessor** | Pointer to [**PatchedImageProcessorModuleRequest**](PatchedImageProcessorModuleRequest.md) |  | [optional] 

## Methods

### NewPatchedApplicationModulesRequest

`func NewPatchedApplicationModulesRequest() *PatchedApplicationModulesRequest`

NewPatchedApplicationModulesRequest instantiates a new PatchedApplicationModulesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedApplicationModulesRequestWithDefaults

`func NewPatchedApplicationModulesRequestWithDefaults() *PatchedApplicationModulesRequest`

NewPatchedApplicationModulesRequestWithDefaults instantiates a new PatchedApplicationModulesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCache

`func (o *PatchedApplicationModulesRequest) GetCache() PatchedCacheModuleRequest`

GetCache returns the Cache field if non-nil, zero value otherwise.

### GetCacheOk

`func (o *PatchedApplicationModulesRequest) GetCacheOk() (*PatchedCacheModuleRequest, bool)`

GetCacheOk returns a tuple with the Cache field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCache

`func (o *PatchedApplicationModulesRequest) SetCache(v PatchedCacheModuleRequest)`

SetCache sets Cache field to given value.

### HasCache

`func (o *PatchedApplicationModulesRequest) HasCache() bool`

HasCache returns a boolean if a field has been set.

### GetFunctions

`func (o *PatchedApplicationModulesRequest) GetFunctions() PatchedFunctionModuleRequest`

GetFunctions returns the Functions field if non-nil, zero value otherwise.

### GetFunctionsOk

`func (o *PatchedApplicationModulesRequest) GetFunctionsOk() (*PatchedFunctionModuleRequest, bool)`

GetFunctionsOk returns a tuple with the Functions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFunctions

`func (o *PatchedApplicationModulesRequest) SetFunctions(v PatchedFunctionModuleRequest)`

SetFunctions sets Functions field to given value.

### HasFunctions

`func (o *PatchedApplicationModulesRequest) HasFunctions() bool`

HasFunctions returns a boolean if a field has been set.

### GetApplicationAccelerator

`func (o *PatchedApplicationModulesRequest) GetApplicationAccelerator() PatchedApplicationAcceleratorModuleRequest`

GetApplicationAccelerator returns the ApplicationAccelerator field if non-nil, zero value otherwise.

### GetApplicationAcceleratorOk

`func (o *PatchedApplicationModulesRequest) GetApplicationAcceleratorOk() (*PatchedApplicationAcceleratorModuleRequest, bool)`

GetApplicationAcceleratorOk returns a tuple with the ApplicationAccelerator field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApplicationAccelerator

`func (o *PatchedApplicationModulesRequest) SetApplicationAccelerator(v PatchedApplicationAcceleratorModuleRequest)`

SetApplicationAccelerator sets ApplicationAccelerator field to given value.

### HasApplicationAccelerator

`func (o *PatchedApplicationModulesRequest) HasApplicationAccelerator() bool`

HasApplicationAccelerator returns a boolean if a field has been set.

### GetImageProcessor

`func (o *PatchedApplicationModulesRequest) GetImageProcessor() PatchedImageProcessorModuleRequest`

GetImageProcessor returns the ImageProcessor field if non-nil, zero value otherwise.

### GetImageProcessorOk

`func (o *PatchedApplicationModulesRequest) GetImageProcessorOk() (*PatchedImageProcessorModuleRequest, bool)`

GetImageProcessorOk returns a tuple with the ImageProcessor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImageProcessor

`func (o *PatchedApplicationModulesRequest) SetImageProcessor(v PatchedImageProcessorModuleRequest)`

SetImageProcessor sets ImageProcessor field to given value.

### HasImageProcessor

`func (o *PatchedApplicationModulesRequest) HasImageProcessor() bool`

HasImageProcessor returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


