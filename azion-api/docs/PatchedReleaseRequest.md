# PatchedReleaseRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Resources** | Pointer to [**[]PatchedReleaseRequestResourcesInner**](PatchedReleaseRequestResourcesInner.md) |  | [optional] 
**Origin** | Pointer to [**AccountReleaseOrigin**](AccountReleaseOrigin.md) |  | [optional] 

## Methods

### NewPatchedReleaseRequest

`func NewPatchedReleaseRequest() *PatchedReleaseRequest`

NewPatchedReleaseRequest instantiates a new PatchedReleaseRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedReleaseRequestWithDefaults

`func NewPatchedReleaseRequestWithDefaults() *PatchedReleaseRequest`

NewPatchedReleaseRequestWithDefaults instantiates a new PatchedReleaseRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetResources

`func (o *PatchedReleaseRequest) GetResources() []PatchedReleaseRequestResourcesInner`

GetResources returns the Resources field if non-nil, zero value otherwise.

### GetResourcesOk

`func (o *PatchedReleaseRequest) GetResourcesOk() (*[]PatchedReleaseRequestResourcesInner, bool)`

GetResourcesOk returns a tuple with the Resources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResources

`func (o *PatchedReleaseRequest) SetResources(v []PatchedReleaseRequestResourcesInner)`

SetResources sets Resources field to given value.

### HasResources

`func (o *PatchedReleaseRequest) HasResources() bool`

HasResources returns a boolean if a field has been set.

### GetOrigin

`func (o *PatchedReleaseRequest) GetOrigin() AccountReleaseOrigin`

GetOrigin returns the Origin field if non-nil, zero value otherwise.

### GetOriginOk

`func (o *PatchedReleaseRequest) GetOriginOk() (*AccountReleaseOrigin, bool)`

GetOriginOk returns a tuple with the Origin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrigin

`func (o *PatchedReleaseRequest) SetOrigin(v AccountReleaseOrigin)`

SetOrigin sets Origin field to given value.

### HasOrigin

`func (o *PatchedReleaseRequest) HasOrigin() bool`

HasOrigin returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


