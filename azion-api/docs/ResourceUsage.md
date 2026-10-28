# ResourceUsage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DeploymentId** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**VersionState** | Pointer to **string** | * &#x60;draft&#x60; - draft * &#x60;queued&#x60; - queued * &#x60;building&#x60; - building * &#x60;ready&#x60; - ready * &#x60;error&#x60; - error * &#x60;canceled&#x60; - canceled * &#x60;archiving&#x60; - archiving * &#x60;archived&#x60; - archived * &#x60;deleting&#x60; - deleting * &#x60;deleted&#x60; - deleted | [optional] 
**DeploymentPolicy** | Pointer to **string** | * &#x60;single_version&#x60; - single_version * &#x60;versioned_urls&#x60; - versioned_urls | [optional] 
**Resources** | Pointer to [**[]ResourceUsageResourcesInner**](ResourceUsageResourcesInner.md) |  | [optional] 

## Methods

### NewResourceUsage

`func NewResourceUsage() *ResourceUsage`

NewResourceUsage instantiates a new ResourceUsage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResourceUsageWithDefaults

`func NewResourceUsageWithDefaults() *ResourceUsage`

NewResourceUsageWithDefaults instantiates a new ResourceUsage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDeploymentId

`func (o *ResourceUsage) GetDeploymentId() string`

GetDeploymentId returns the DeploymentId field if non-nil, zero value otherwise.

### GetDeploymentIdOk

`func (o *ResourceUsage) GetDeploymentIdOk() (*string, bool)`

GetDeploymentIdOk returns a tuple with the DeploymentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentId

`func (o *ResourceUsage) SetDeploymentId(v string)`

SetDeploymentId sets DeploymentId field to given value.

### HasDeploymentId

`func (o *ResourceUsage) HasDeploymentId() bool`

HasDeploymentId returns a boolean if a field has been set.

### GetName

`func (o *ResourceUsage) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ResourceUsage) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ResourceUsage) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ResourceUsage) HasName() bool`

HasName returns a boolean if a field has been set.

### GetVersionState

`func (o *ResourceUsage) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *ResourceUsage) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *ResourceUsage) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *ResourceUsage) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetDeploymentPolicy

`func (o *ResourceUsage) GetDeploymentPolicy() string`

GetDeploymentPolicy returns the DeploymentPolicy field if non-nil, zero value otherwise.

### GetDeploymentPolicyOk

`func (o *ResourceUsage) GetDeploymentPolicyOk() (*string, bool)`

GetDeploymentPolicyOk returns a tuple with the DeploymentPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentPolicy

`func (o *ResourceUsage) SetDeploymentPolicy(v string)`

SetDeploymentPolicy sets DeploymentPolicy field to given value.

### HasDeploymentPolicy

`func (o *ResourceUsage) HasDeploymentPolicy() bool`

HasDeploymentPolicy returns a boolean if a field has been set.

### GetResources

`func (o *ResourceUsage) GetResources() []ResourceUsageResourcesInner`

GetResources returns the Resources field if non-nil, zero value otherwise.

### GetResourcesOk

`func (o *ResourceUsage) GetResourcesOk() (*[]ResourceUsageResourcesInner, bool)`

GetResourcesOk returns a tuple with the Resources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResources

`func (o *ResourceUsage) SetResources(v []ResourceUsageResourcesInner)`

SetResources sets Resources field to given value.

### HasResources

`func (o *ResourceUsage) HasResources() bool`

HasResources returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


