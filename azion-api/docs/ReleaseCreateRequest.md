# ReleaseCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Resources** | Pointer to [**[]PatchedReleaseRequestResourcesInner**](PatchedReleaseRequestResourcesInner.md) |  | [optional] 
**Origin** | Pointer to [**AccountReleaseOrigin**](AccountReleaseOrigin.md) |  | [optional] 

## Methods

### NewReleaseCreateRequest

`func NewReleaseCreateRequest() *ReleaseCreateRequest`

NewReleaseCreateRequest instantiates a new ReleaseCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReleaseCreateRequestWithDefaults

`func NewReleaseCreateRequestWithDefaults() *ReleaseCreateRequest`

NewReleaseCreateRequestWithDefaults instantiates a new ReleaseCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetResources

`func (o *ReleaseCreateRequest) GetResources() []PatchedReleaseRequestResourcesInner`

GetResources returns the Resources field if non-nil, zero value otherwise.

### GetResourcesOk

`func (o *ReleaseCreateRequest) GetResourcesOk() (*[]PatchedReleaseRequestResourcesInner, bool)`

GetResourcesOk returns a tuple with the Resources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResources

`func (o *ReleaseCreateRequest) SetResources(v []PatchedReleaseRequestResourcesInner)`

SetResources sets Resources field to given value.

### HasResources

`func (o *ReleaseCreateRequest) HasResources() bool`

HasResources returns a boolean if a field has been set.

### GetOrigin

`func (o *ReleaseCreateRequest) GetOrigin() AccountReleaseOrigin`

GetOrigin returns the Origin field if non-nil, zero value otherwise.

### GetOriginOk

`func (o *ReleaseCreateRequest) GetOriginOk() (*AccountReleaseOrigin, bool)`

GetOriginOk returns a tuple with the Origin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrigin

`func (o *ReleaseCreateRequest) SetOrigin(v AccountReleaseOrigin)`

SetOrigin sets Origin field to given value.

### HasOrigin

`func (o *ReleaseCreateRequest) HasOrigin() bool`

HasOrigin returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


