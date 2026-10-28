# EnvironmentRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Description** | **NullableString** |  | 
**LogVerbosity** | **string** | * &#x60;normal&#x60; - normal * &#x60;verbose&#x60; - verbose | 
**RobotsPolicy** | **string** | * &#x60;index&#x60; - index * &#x60;noindex&#x60; - noindex * &#x60;respect_origin&#x60; - respect_origin | 
**Protection** | [**EnvironmentCreateRequestProtection**](EnvironmentCreateRequestProtection.md) |  | 
**BranchTracking** | [**NullableEnvironmentBranchTracking**](EnvironmentBranchTracking.md) |  | 
**DeploymentPolicy** | Pointer to **string** | * &#x60;single_version&#x60; - single_version * &#x60;versioned_urls&#x60; - versioned_urls | [optional] 

## Methods

### NewEnvironmentRequest

`func NewEnvironmentRequest(name string, description NullableString, logVerbosity string, robotsPolicy string, protection EnvironmentCreateRequestProtection, branchTracking NullableEnvironmentBranchTracking, ) *EnvironmentRequest`

NewEnvironmentRequest instantiates a new EnvironmentRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEnvironmentRequestWithDefaults

`func NewEnvironmentRequestWithDefaults() *EnvironmentRequest`

NewEnvironmentRequestWithDefaults instantiates a new EnvironmentRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *EnvironmentRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *EnvironmentRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *EnvironmentRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *EnvironmentRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *EnvironmentRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *EnvironmentRequest) SetDescription(v string)`

SetDescription sets Description field to given value.


### SetDescriptionNil

`func (o *EnvironmentRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *EnvironmentRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetLogVerbosity

`func (o *EnvironmentRequest) GetLogVerbosity() string`

GetLogVerbosity returns the LogVerbosity field if non-nil, zero value otherwise.

### GetLogVerbosityOk

`func (o *EnvironmentRequest) GetLogVerbosityOk() (*string, bool)`

GetLogVerbosityOk returns a tuple with the LogVerbosity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogVerbosity

`func (o *EnvironmentRequest) SetLogVerbosity(v string)`

SetLogVerbosity sets LogVerbosity field to given value.


### GetRobotsPolicy

`func (o *EnvironmentRequest) GetRobotsPolicy() string`

GetRobotsPolicy returns the RobotsPolicy field if non-nil, zero value otherwise.

### GetRobotsPolicyOk

`func (o *EnvironmentRequest) GetRobotsPolicyOk() (*string, bool)`

GetRobotsPolicyOk returns a tuple with the RobotsPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRobotsPolicy

`func (o *EnvironmentRequest) SetRobotsPolicy(v string)`

SetRobotsPolicy sets RobotsPolicy field to given value.


### GetProtection

`func (o *EnvironmentRequest) GetProtection() EnvironmentCreateRequestProtection`

GetProtection returns the Protection field if non-nil, zero value otherwise.

### GetProtectionOk

`func (o *EnvironmentRequest) GetProtectionOk() (*EnvironmentCreateRequestProtection, bool)`

GetProtectionOk returns a tuple with the Protection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProtection

`func (o *EnvironmentRequest) SetProtection(v EnvironmentCreateRequestProtection)`

SetProtection sets Protection field to given value.


### GetBranchTracking

`func (o *EnvironmentRequest) GetBranchTracking() EnvironmentBranchTracking`

GetBranchTracking returns the BranchTracking field if non-nil, zero value otherwise.

### GetBranchTrackingOk

`func (o *EnvironmentRequest) GetBranchTrackingOk() (*EnvironmentBranchTracking, bool)`

GetBranchTrackingOk returns a tuple with the BranchTracking field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranchTracking

`func (o *EnvironmentRequest) SetBranchTracking(v EnvironmentBranchTracking)`

SetBranchTracking sets BranchTracking field to given value.


### SetBranchTrackingNil

`func (o *EnvironmentRequest) SetBranchTrackingNil(b bool)`

 SetBranchTrackingNil sets the value for BranchTracking to be an explicit nil

### UnsetBranchTracking
`func (o *EnvironmentRequest) UnsetBranchTracking()`

UnsetBranchTracking ensures that no value is present for BranchTracking, not even an explicit nil
### GetDeploymentPolicy

`func (o *EnvironmentRequest) GetDeploymentPolicy() string`

GetDeploymentPolicy returns the DeploymentPolicy field if non-nil, zero value otherwise.

### GetDeploymentPolicyOk

`func (o *EnvironmentRequest) GetDeploymentPolicyOk() (*string, bool)`

GetDeploymentPolicyOk returns a tuple with the DeploymentPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentPolicy

`func (o *EnvironmentRequest) SetDeploymentPolicy(v string)`

SetDeploymentPolicy sets DeploymentPolicy field to given value.

### HasDeploymentPolicy

`func (o *EnvironmentRequest) HasDeploymentPolicy() bool`

HasDeploymentPolicy returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


