# ReleaseRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Resources** | [**[]ReleaseCreateRequestResourcesInner**](ReleaseCreateRequestResourcesInner.md) |  | 
**Origin** | [**ReleaseOrigin**](ReleaseOrigin.md) |  | 

## Methods

### NewReleaseRequest

`func NewReleaseRequest(resources []ReleaseCreateRequestResourcesInner, origin ReleaseOrigin, ) *ReleaseRequest`

NewReleaseRequest instantiates a new ReleaseRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReleaseRequestWithDefaults

`func NewReleaseRequestWithDefaults() *ReleaseRequest`

NewReleaseRequestWithDefaults instantiates a new ReleaseRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetResources

`func (o *ReleaseRequest) GetResources() []ReleaseCreateRequestResourcesInner`

GetResources returns the Resources field if non-nil, zero value otherwise.

### GetResourcesOk

`func (o *ReleaseRequest) GetResourcesOk() (*[]ReleaseCreateRequestResourcesInner, bool)`

GetResourcesOk returns a tuple with the Resources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResources

`func (o *ReleaseRequest) SetResources(v []ReleaseCreateRequestResourcesInner)`

SetResources sets Resources field to given value.


### GetOrigin

`func (o *ReleaseRequest) GetOrigin() ReleaseOrigin`

GetOrigin returns the Origin field if non-nil, zero value otherwise.

### GetOriginOk

`func (o *ReleaseRequest) GetOriginOk() (*ReleaseOrigin, bool)`

GetOriginOk returns a tuple with the Origin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrigin

`func (o *ReleaseRequest) SetOrigin(v ReleaseOrigin)`

SetOrigin sets Origin field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


