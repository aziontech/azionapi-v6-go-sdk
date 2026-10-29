# ResourceHierarchyResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DeploymentId** | **string** |  | 
**ActiveReleaseId** | **NullableString** |  | 
**Resources** | [**ResourceHierarchyResponseDataResources**](ResourceHierarchyResponseDataResources.md) |  | 

## Methods

### NewResourceHierarchyResponseData

`func NewResourceHierarchyResponseData(deploymentId string, activeReleaseId NullableString, resources ResourceHierarchyResponseDataResources, ) *ResourceHierarchyResponseData`

NewResourceHierarchyResponseData instantiates a new ResourceHierarchyResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResourceHierarchyResponseDataWithDefaults

`func NewResourceHierarchyResponseDataWithDefaults() *ResourceHierarchyResponseData`

NewResourceHierarchyResponseDataWithDefaults instantiates a new ResourceHierarchyResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDeploymentId

`func (o *ResourceHierarchyResponseData) GetDeploymentId() string`

GetDeploymentId returns the DeploymentId field if non-nil, zero value otherwise.

### GetDeploymentIdOk

`func (o *ResourceHierarchyResponseData) GetDeploymentIdOk() (*string, bool)`

GetDeploymentIdOk returns a tuple with the DeploymentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentId

`func (o *ResourceHierarchyResponseData) SetDeploymentId(v string)`

SetDeploymentId sets DeploymentId field to given value.


### GetActiveReleaseId

`func (o *ResourceHierarchyResponseData) GetActiveReleaseId() string`

GetActiveReleaseId returns the ActiveReleaseId field if non-nil, zero value otherwise.

### GetActiveReleaseIdOk

`func (o *ResourceHierarchyResponseData) GetActiveReleaseIdOk() (*string, bool)`

GetActiveReleaseIdOk returns a tuple with the ActiveReleaseId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActiveReleaseId

`func (o *ResourceHierarchyResponseData) SetActiveReleaseId(v string)`

SetActiveReleaseId sets ActiveReleaseId field to given value.


### SetActiveReleaseIdNil

`func (o *ResourceHierarchyResponseData) SetActiveReleaseIdNil(b bool)`

 SetActiveReleaseIdNil sets the value for ActiveReleaseId to be an explicit nil

### UnsetActiveReleaseId
`func (o *ResourceHierarchyResponseData) UnsetActiveReleaseId()`

UnsetActiveReleaseId ensures that no value is present for ActiveReleaseId, not even an explicit nil
### GetResources

`func (o *ResourceHierarchyResponseData) GetResources() ResourceHierarchyResponseDataResources`

GetResources returns the Resources field if non-nil, zero value otherwise.

### GetResourcesOk

`func (o *ResourceHierarchyResponseData) GetResourcesOk() (*ResourceHierarchyResponseDataResources, bool)`

GetResourcesOk returns a tuple with the Resources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResources

`func (o *ResourceHierarchyResponseData) SetResources(v ResourceHierarchyResponseDataResources)`

SetResources sets Resources field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


