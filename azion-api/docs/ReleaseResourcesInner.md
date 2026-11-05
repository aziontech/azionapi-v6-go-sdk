# ReleaseResourcesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ResourceId** | **NullableInt64** |  | 
**ResourceType** | **string** |  | 
**VersionId** | **NullableString** |  | 

## Methods

### NewReleaseResourcesInner

`func NewReleaseResourcesInner(resourceId NullableInt64, resourceType string, versionId NullableString, ) *ReleaseResourcesInner`

NewReleaseResourcesInner instantiates a new ReleaseResourcesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReleaseResourcesInnerWithDefaults

`func NewReleaseResourcesInnerWithDefaults() *ReleaseResourcesInner`

NewReleaseResourcesInnerWithDefaults instantiates a new ReleaseResourcesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetResourceId

`func (o *ReleaseResourcesInner) GetResourceId() int64`

GetResourceId returns the ResourceId field if non-nil, zero value otherwise.

### GetResourceIdOk

`func (o *ReleaseResourcesInner) GetResourceIdOk() (*int64, bool)`

GetResourceIdOk returns a tuple with the ResourceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResourceId

`func (o *ReleaseResourcesInner) SetResourceId(v int64)`

SetResourceId sets ResourceId field to given value.


### SetResourceIdNil

`func (o *ReleaseResourcesInner) SetResourceIdNil(b bool)`

 SetResourceIdNil sets the value for ResourceId to be an explicit nil

### UnsetResourceId
`func (o *ReleaseResourcesInner) UnsetResourceId()`

UnsetResourceId ensures that no value is present for ResourceId, not even an explicit nil
### GetResourceType

`func (o *ReleaseResourcesInner) GetResourceType() string`

GetResourceType returns the ResourceType field if non-nil, zero value otherwise.

### GetResourceTypeOk

`func (o *ReleaseResourcesInner) GetResourceTypeOk() (*string, bool)`

GetResourceTypeOk returns a tuple with the ResourceType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResourceType

`func (o *ReleaseResourcesInner) SetResourceType(v string)`

SetResourceType sets ResourceType field to given value.


### GetVersionId

`func (o *ReleaseResourcesInner) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *ReleaseResourcesInner) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *ReleaseResourcesInner) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.


### SetVersionIdNil

`func (o *ReleaseResourcesInner) SetVersionIdNil(b bool)`

 SetVersionIdNil sets the value for VersionId to be an explicit nil

### UnsetVersionId
`func (o *ReleaseResourcesInner) UnsetVersionId()`

UnsetVersionId ensures that no value is present for VersionId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


