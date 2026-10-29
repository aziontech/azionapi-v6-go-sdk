# EnvironmentCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**DeploymentPolicy** | **string** | * &#x60;single_version&#x60; - single_version * &#x60;versioned_urls&#x60; - versioned_urls | 
**LogVerbosity** | Pointer to **string** | * &#x60;normal&#x60; - normal * &#x60;verbose&#x60; - verbose | [optional] 
**RobotsPolicy** | Pointer to **string** | * &#x60;index&#x60; - index * &#x60;noindex&#x60; - noindex * &#x60;respect_origin&#x60; - respect_origin | [optional] 
**Protection** | Pointer to [**EnvironmentCreateRequestProtection**](EnvironmentCreateRequestProtection.md) |  | [optional] 
**BranchTracking** | Pointer to [**NullableEnvironmentBranchTracking**](EnvironmentBranchTracking.md) |  | [optional] 

## Methods

### NewEnvironmentCreateRequest

`func NewEnvironmentCreateRequest(name string, deploymentPolicy string, ) *EnvironmentCreateRequest`

NewEnvironmentCreateRequest instantiates a new EnvironmentCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEnvironmentCreateRequestWithDefaults

`func NewEnvironmentCreateRequestWithDefaults() *EnvironmentCreateRequest`

NewEnvironmentCreateRequestWithDefaults instantiates a new EnvironmentCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *EnvironmentCreateRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *EnvironmentCreateRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *EnvironmentCreateRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *EnvironmentCreateRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *EnvironmentCreateRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *EnvironmentCreateRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *EnvironmentCreateRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *EnvironmentCreateRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *EnvironmentCreateRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetDeploymentPolicy

`func (o *EnvironmentCreateRequest) GetDeploymentPolicy() string`

GetDeploymentPolicy returns the DeploymentPolicy field if non-nil, zero value otherwise.

### GetDeploymentPolicyOk

`func (o *EnvironmentCreateRequest) GetDeploymentPolicyOk() (*string, bool)`

GetDeploymentPolicyOk returns a tuple with the DeploymentPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentPolicy

`func (o *EnvironmentCreateRequest) SetDeploymentPolicy(v string)`

SetDeploymentPolicy sets DeploymentPolicy field to given value.


### GetLogVerbosity

`func (o *EnvironmentCreateRequest) GetLogVerbosity() string`

GetLogVerbosity returns the LogVerbosity field if non-nil, zero value otherwise.

### GetLogVerbosityOk

`func (o *EnvironmentCreateRequest) GetLogVerbosityOk() (*string, bool)`

GetLogVerbosityOk returns a tuple with the LogVerbosity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogVerbosity

`func (o *EnvironmentCreateRequest) SetLogVerbosity(v string)`

SetLogVerbosity sets LogVerbosity field to given value.

### HasLogVerbosity

`func (o *EnvironmentCreateRequest) HasLogVerbosity() bool`

HasLogVerbosity returns a boolean if a field has been set.

### GetRobotsPolicy

`func (o *EnvironmentCreateRequest) GetRobotsPolicy() string`

GetRobotsPolicy returns the RobotsPolicy field if non-nil, zero value otherwise.

### GetRobotsPolicyOk

`func (o *EnvironmentCreateRequest) GetRobotsPolicyOk() (*string, bool)`

GetRobotsPolicyOk returns a tuple with the RobotsPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRobotsPolicy

`func (o *EnvironmentCreateRequest) SetRobotsPolicy(v string)`

SetRobotsPolicy sets RobotsPolicy field to given value.

### HasRobotsPolicy

`func (o *EnvironmentCreateRequest) HasRobotsPolicy() bool`

HasRobotsPolicy returns a boolean if a field has been set.

### GetProtection

`func (o *EnvironmentCreateRequest) GetProtection() EnvironmentCreateRequestProtection`

GetProtection returns the Protection field if non-nil, zero value otherwise.

### GetProtectionOk

`func (o *EnvironmentCreateRequest) GetProtectionOk() (*EnvironmentCreateRequestProtection, bool)`

GetProtectionOk returns a tuple with the Protection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProtection

`func (o *EnvironmentCreateRequest) SetProtection(v EnvironmentCreateRequestProtection)`

SetProtection sets Protection field to given value.

### HasProtection

`func (o *EnvironmentCreateRequest) HasProtection() bool`

HasProtection returns a boolean if a field has been set.

### GetBranchTracking

`func (o *EnvironmentCreateRequest) GetBranchTracking() EnvironmentBranchTracking`

GetBranchTracking returns the BranchTracking field if non-nil, zero value otherwise.

### GetBranchTrackingOk

`func (o *EnvironmentCreateRequest) GetBranchTrackingOk() (*EnvironmentBranchTracking, bool)`

GetBranchTrackingOk returns a tuple with the BranchTracking field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranchTracking

`func (o *EnvironmentCreateRequest) SetBranchTracking(v EnvironmentBranchTracking)`

SetBranchTracking sets BranchTracking field to given value.

### HasBranchTracking

`func (o *EnvironmentCreateRequest) HasBranchTracking() bool`

HasBranchTracking returns a boolean if a field has been set.

### SetBranchTrackingNil

`func (o *EnvironmentCreateRequest) SetBranchTrackingNil(b bool)`

 SetBranchTrackingNil sets the value for BranchTracking to be an explicit nil

### UnsetBranchTracking
`func (o *EnvironmentCreateRequest) UnsetBranchTracking()`

UnsetBranchTracking ensures that no value is present for BranchTracking, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


