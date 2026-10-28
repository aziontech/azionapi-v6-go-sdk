# PatchedScopeItemRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ResourceType** | Pointer to **string** | * &#x60;global&#x60; - global * &#x60;environment&#x60; - environment * &#x60;deployment&#x60; - deployment * &#x60;application&#x60; - application * &#x60;firewall&#x60; - firewall | [optional] 
**ResourceId** | Pointer to **string** |  | [optional] 

## Methods

### NewPatchedScopeItemRequest

`func NewPatchedScopeItemRequest() *PatchedScopeItemRequest`

NewPatchedScopeItemRequest instantiates a new PatchedScopeItemRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedScopeItemRequestWithDefaults

`func NewPatchedScopeItemRequestWithDefaults() *PatchedScopeItemRequest`

NewPatchedScopeItemRequestWithDefaults instantiates a new PatchedScopeItemRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetResourceType

`func (o *PatchedScopeItemRequest) GetResourceType() string`

GetResourceType returns the ResourceType field if non-nil, zero value otherwise.

### GetResourceTypeOk

`func (o *PatchedScopeItemRequest) GetResourceTypeOk() (*string, bool)`

GetResourceTypeOk returns a tuple with the ResourceType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResourceType

`func (o *PatchedScopeItemRequest) SetResourceType(v string)`

SetResourceType sets ResourceType field to given value.

### HasResourceType

`func (o *PatchedScopeItemRequest) HasResourceType() bool`

HasResourceType returns a boolean if a field has been set.

### GetResourceId

`func (o *PatchedScopeItemRequest) GetResourceId() string`

GetResourceId returns the ResourceId field if non-nil, zero value otherwise.

### GetResourceIdOk

`func (o *PatchedScopeItemRequest) GetResourceIdOk() (*string, bool)`

GetResourceIdOk returns a tuple with the ResourceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResourceId

`func (o *PatchedScopeItemRequest) SetResourceId(v string)`

SetResourceId sets ResourceId field to given value.

### HasResourceId

`func (o *PatchedScopeItemRequest) HasResourceId() bool`

HasResourceId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


