# BuildAndActivateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Resources** | [**[]BuildAndActivateRequestResourcesInner**](BuildAndActivateRequestResourcesInner.md) |  | 
**Origin** | Pointer to [**ReleaseOrigin**](ReleaseOrigin.md) |  | [optional] 
**DeploymentVersionId** | Pointer to **string** |  | [optional] 

## Methods

### NewBuildAndActivateRequest

`func NewBuildAndActivateRequest(resources []BuildAndActivateRequestResourcesInner, ) *BuildAndActivateRequest`

NewBuildAndActivateRequest instantiates a new BuildAndActivateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBuildAndActivateRequestWithDefaults

`func NewBuildAndActivateRequestWithDefaults() *BuildAndActivateRequest`

NewBuildAndActivateRequestWithDefaults instantiates a new BuildAndActivateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetResources

`func (o *BuildAndActivateRequest) GetResources() []BuildAndActivateRequestResourcesInner`

GetResources returns the Resources field if non-nil, zero value otherwise.

### GetResourcesOk

`func (o *BuildAndActivateRequest) GetResourcesOk() (*[]BuildAndActivateRequestResourcesInner, bool)`

GetResourcesOk returns a tuple with the Resources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResources

`func (o *BuildAndActivateRequest) SetResources(v []BuildAndActivateRequestResourcesInner)`

SetResources sets Resources field to given value.


### GetOrigin

`func (o *BuildAndActivateRequest) GetOrigin() ReleaseOrigin`

GetOrigin returns the Origin field if non-nil, zero value otherwise.

### GetOriginOk

`func (o *BuildAndActivateRequest) GetOriginOk() (*ReleaseOrigin, bool)`

GetOriginOk returns a tuple with the Origin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrigin

`func (o *BuildAndActivateRequest) SetOrigin(v ReleaseOrigin)`

SetOrigin sets Origin field to given value.

### HasOrigin

`func (o *BuildAndActivateRequest) HasOrigin() bool`

HasOrigin returns a boolean if a field has been set.

### GetDeploymentVersionId

`func (o *BuildAndActivateRequest) GetDeploymentVersionId() string`

GetDeploymentVersionId returns the DeploymentVersionId field if non-nil, zero value otherwise.

### GetDeploymentVersionIdOk

`func (o *BuildAndActivateRequest) GetDeploymentVersionIdOk() (*string, bool)`

GetDeploymentVersionIdOk returns a tuple with the DeploymentVersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentVersionId

`func (o *BuildAndActivateRequest) SetDeploymentVersionId(v string)`

SetDeploymentVersionId sets DeploymentVersionId field to given value.

### HasDeploymentVersionId

`func (o *BuildAndActivateRequest) HasDeploymentVersionId() bool`

HasDeploymentVersionId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


