# ResourceUsageResourcesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ResourceType** | **string** |  | 
**ResourceId** | **string** |  | 
**ResourceVersion** | **NullableString** |  | 
**ProductVersion** | **NullableString** |  | 
**ReleaseId** | **string** |  | 
**TrafficRole** | **string** | * &#x60;ACTIVE&#x60; - ACTIVE * &#x60;CANDIDATE&#x60; - CANDIDATE * &#x60;VALID_URL&#x60; - VALID_URL * &#x60;INACTIVE&#x60; - INACTIVE | 

## Methods

### NewResourceUsageResourcesInner

`func NewResourceUsageResourcesInner(resourceType string, resourceId string, resourceVersion NullableString, productVersion NullableString, releaseId string, trafficRole string, ) *ResourceUsageResourcesInner`

NewResourceUsageResourcesInner instantiates a new ResourceUsageResourcesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResourceUsageResourcesInnerWithDefaults

`func NewResourceUsageResourcesInnerWithDefaults() *ResourceUsageResourcesInner`

NewResourceUsageResourcesInnerWithDefaults instantiates a new ResourceUsageResourcesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetResourceType

`func (o *ResourceUsageResourcesInner) GetResourceType() string`

GetResourceType returns the ResourceType field if non-nil, zero value otherwise.

### GetResourceTypeOk

`func (o *ResourceUsageResourcesInner) GetResourceTypeOk() (*string, bool)`

GetResourceTypeOk returns a tuple with the ResourceType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResourceType

`func (o *ResourceUsageResourcesInner) SetResourceType(v string)`

SetResourceType sets ResourceType field to given value.


### GetResourceId

`func (o *ResourceUsageResourcesInner) GetResourceId() string`

GetResourceId returns the ResourceId field if non-nil, zero value otherwise.

### GetResourceIdOk

`func (o *ResourceUsageResourcesInner) GetResourceIdOk() (*string, bool)`

GetResourceIdOk returns a tuple with the ResourceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResourceId

`func (o *ResourceUsageResourcesInner) SetResourceId(v string)`

SetResourceId sets ResourceId field to given value.


### GetResourceVersion

`func (o *ResourceUsageResourcesInner) GetResourceVersion() string`

GetResourceVersion returns the ResourceVersion field if non-nil, zero value otherwise.

### GetResourceVersionOk

`func (o *ResourceUsageResourcesInner) GetResourceVersionOk() (*string, bool)`

GetResourceVersionOk returns a tuple with the ResourceVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResourceVersion

`func (o *ResourceUsageResourcesInner) SetResourceVersion(v string)`

SetResourceVersion sets ResourceVersion field to given value.


### SetResourceVersionNil

`func (o *ResourceUsageResourcesInner) SetResourceVersionNil(b bool)`

 SetResourceVersionNil sets the value for ResourceVersion to be an explicit nil

### UnsetResourceVersion
`func (o *ResourceUsageResourcesInner) UnsetResourceVersion()`

UnsetResourceVersion ensures that no value is present for ResourceVersion, not even an explicit nil
### GetProductVersion

`func (o *ResourceUsageResourcesInner) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *ResourceUsageResourcesInner) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *ResourceUsageResourcesInner) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.


### SetProductVersionNil

`func (o *ResourceUsageResourcesInner) SetProductVersionNil(b bool)`

 SetProductVersionNil sets the value for ProductVersion to be an explicit nil

### UnsetProductVersion
`func (o *ResourceUsageResourcesInner) UnsetProductVersion()`

UnsetProductVersion ensures that no value is present for ProductVersion, not even an explicit nil
### GetReleaseId

`func (o *ResourceUsageResourcesInner) GetReleaseId() string`

GetReleaseId returns the ReleaseId field if non-nil, zero value otherwise.

### GetReleaseIdOk

`func (o *ResourceUsageResourcesInner) GetReleaseIdOk() (*string, bool)`

GetReleaseIdOk returns a tuple with the ReleaseId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReleaseId

`func (o *ResourceUsageResourcesInner) SetReleaseId(v string)`

SetReleaseId sets ReleaseId field to given value.


### GetTrafficRole

`func (o *ResourceUsageResourcesInner) GetTrafficRole() string`

GetTrafficRole returns the TrafficRole field if non-nil, zero value otherwise.

### GetTrafficRoleOk

`func (o *ResourceUsageResourcesInner) GetTrafficRoleOk() (*string, bool)`

GetTrafficRoleOk returns a tuple with the TrafficRole field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrafficRole

`func (o *ResourceUsageResourcesInner) SetTrafficRole(v string)`

SetTrafficRole sets TrafficRole field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


