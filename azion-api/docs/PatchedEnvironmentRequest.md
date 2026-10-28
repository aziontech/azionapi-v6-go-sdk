# PatchedEnvironmentRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **NullableString** |  | [optional] 
**DeploymentPolicy** | Pointer to **string** | * &#x60;single_version&#x60; - single_version * &#x60;versioned_urls&#x60; - versioned_urls | [optional] 
**LogVerbosity** | Pointer to **string** | * &#x60;normal&#x60; - normal * &#x60;verbose&#x60; - verbose | [optional] 
**RobotsPolicy** | Pointer to **string** | * &#x60;index&#x60; - index * &#x60;noindex&#x60; - noindex * &#x60;respect_origin&#x60; - respect_origin | [optional] 
**Protection** | Pointer to [**EnvironmentCreateRequestProtection**](EnvironmentCreateRequestProtection.md) |  | [optional] 
**BranchTracking** | Pointer to [**NullableEnvironmentBranchTracking**](EnvironmentBranchTracking.md) |  | [optional] 

## Methods

### NewPatchedEnvironmentRequest

`func NewPatchedEnvironmentRequest() *PatchedEnvironmentRequest`

NewPatchedEnvironmentRequest instantiates a new PatchedEnvironmentRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedEnvironmentRequestWithDefaults

`func NewPatchedEnvironmentRequestWithDefaults() *PatchedEnvironmentRequest`

NewPatchedEnvironmentRequestWithDefaults instantiates a new PatchedEnvironmentRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *PatchedEnvironmentRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *PatchedEnvironmentRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *PatchedEnvironmentRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *PatchedEnvironmentRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *PatchedEnvironmentRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *PatchedEnvironmentRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *PatchedEnvironmentRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *PatchedEnvironmentRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *PatchedEnvironmentRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *PatchedEnvironmentRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetDeploymentPolicy

`func (o *PatchedEnvironmentRequest) GetDeploymentPolicy() string`

GetDeploymentPolicy returns the DeploymentPolicy field if non-nil, zero value otherwise.

### GetDeploymentPolicyOk

`func (o *PatchedEnvironmentRequest) GetDeploymentPolicyOk() (*string, bool)`

GetDeploymentPolicyOk returns a tuple with the DeploymentPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentPolicy

`func (o *PatchedEnvironmentRequest) SetDeploymentPolicy(v string)`

SetDeploymentPolicy sets DeploymentPolicy field to given value.

### HasDeploymentPolicy

`func (o *PatchedEnvironmentRequest) HasDeploymentPolicy() bool`

HasDeploymentPolicy returns a boolean if a field has been set.

### GetLogVerbosity

`func (o *PatchedEnvironmentRequest) GetLogVerbosity() string`

GetLogVerbosity returns the LogVerbosity field if non-nil, zero value otherwise.

### GetLogVerbosityOk

`func (o *PatchedEnvironmentRequest) GetLogVerbosityOk() (*string, bool)`

GetLogVerbosityOk returns a tuple with the LogVerbosity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogVerbosity

`func (o *PatchedEnvironmentRequest) SetLogVerbosity(v string)`

SetLogVerbosity sets LogVerbosity field to given value.

### HasLogVerbosity

`func (o *PatchedEnvironmentRequest) HasLogVerbosity() bool`

HasLogVerbosity returns a boolean if a field has been set.

### GetRobotsPolicy

`func (o *PatchedEnvironmentRequest) GetRobotsPolicy() string`

GetRobotsPolicy returns the RobotsPolicy field if non-nil, zero value otherwise.

### GetRobotsPolicyOk

`func (o *PatchedEnvironmentRequest) GetRobotsPolicyOk() (*string, bool)`

GetRobotsPolicyOk returns a tuple with the RobotsPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRobotsPolicy

`func (o *PatchedEnvironmentRequest) SetRobotsPolicy(v string)`

SetRobotsPolicy sets RobotsPolicy field to given value.

### HasRobotsPolicy

`func (o *PatchedEnvironmentRequest) HasRobotsPolicy() bool`

HasRobotsPolicy returns a boolean if a field has been set.

### GetProtection

`func (o *PatchedEnvironmentRequest) GetProtection() EnvironmentCreateRequestProtection`

GetProtection returns the Protection field if non-nil, zero value otherwise.

### GetProtectionOk

`func (o *PatchedEnvironmentRequest) GetProtectionOk() (*EnvironmentCreateRequestProtection, bool)`

GetProtectionOk returns a tuple with the Protection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProtection

`func (o *PatchedEnvironmentRequest) SetProtection(v EnvironmentCreateRequestProtection)`

SetProtection sets Protection field to given value.

### HasProtection

`func (o *PatchedEnvironmentRequest) HasProtection() bool`

HasProtection returns a boolean if a field has been set.

### GetBranchTracking

`func (o *PatchedEnvironmentRequest) GetBranchTracking() EnvironmentBranchTracking`

GetBranchTracking returns the BranchTracking field if non-nil, zero value otherwise.

### GetBranchTrackingOk

`func (o *PatchedEnvironmentRequest) GetBranchTrackingOk() (*EnvironmentBranchTracking, bool)`

GetBranchTrackingOk returns a tuple with the BranchTracking field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranchTracking

`func (o *PatchedEnvironmentRequest) SetBranchTracking(v EnvironmentBranchTracking)`

SetBranchTracking sets BranchTracking field to given value.

### HasBranchTracking

`func (o *PatchedEnvironmentRequest) HasBranchTracking() bool`

HasBranchTracking returns a boolean if a field has been set.

### SetBranchTrackingNil

`func (o *PatchedEnvironmentRequest) SetBranchTrackingNil(b bool)`

 SetBranchTrackingNil sets the value for BranchTracking to be an explicit nil

### UnsetBranchTracking
`func (o *PatchedEnvironmentRequest) UnsetBranchTracking()`

UnsetBranchTracking ensures that no value is present for BranchTracking, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


