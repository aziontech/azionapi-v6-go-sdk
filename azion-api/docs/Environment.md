# Environment

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**VersionId** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **NullableString** |  | [optional] 
**DeploymentPolicy** | Pointer to **string** | * &#x60;single_version&#x60; - single_version * &#x60;versioned_urls&#x60; - versioned_urls | [optional] 
**LogVerbosity** | Pointer to **string** | * &#x60;normal&#x60; - normal * &#x60;verbose&#x60; - verbose | [optional] 
**RobotsPolicy** | Pointer to **string** | * &#x60;index&#x60; - index * &#x60;noindex&#x60; - noindex * &#x60;respect_origin&#x60; - respect_origin | [optional] 
**Protection** | Pointer to [**EnvironmentProtection**](EnvironmentProtection.md) |  | [optional] 
**BranchTracking** | Pointer to [**NullableEnvironmentBranchTracking**](EnvironmentBranchTracking.md) |  | [optional] 
**VersionState** | Pointer to **string** | * &#x60;draft&#x60; - draft * &#x60;queued&#x60; - queued * &#x60;building&#x60; - building * &#x60;ready&#x60; - ready * &#x60;error&#x60; - error * &#x60;canceled&#x60; - canceled * &#x60;archiving&#x60; - archiving * &#x60;archived&#x60; - archived * &#x60;deleting&#x60; - deleting * &#x60;deleted&#x60; - deleted | [optional] 
**ProductVersion** | Pointer to **string** |  | [optional] 
**ClientId** | Pointer to **string** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**LastModified** | Pointer to **NullableTime** |  | [optional] 
**CreatedBy** | Pointer to **NullableString** |  | [optional] 
**LastEditor** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewEnvironment

`func NewEnvironment() *Environment`

NewEnvironment instantiates a new Environment object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEnvironmentWithDefaults

`func NewEnvironmentWithDefaults() *Environment`

NewEnvironmentWithDefaults instantiates a new Environment object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Environment) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Environment) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Environment) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *Environment) HasId() bool`

HasId returns a boolean if a field has been set.

### GetVersionId

`func (o *Environment) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *Environment) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *Environment) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *Environment) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### GetName

`func (o *Environment) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Environment) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Environment) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *Environment) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *Environment) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *Environment) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *Environment) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *Environment) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *Environment) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *Environment) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetDeploymentPolicy

`func (o *Environment) GetDeploymentPolicy() string`

GetDeploymentPolicy returns the DeploymentPolicy field if non-nil, zero value otherwise.

### GetDeploymentPolicyOk

`func (o *Environment) GetDeploymentPolicyOk() (*string, bool)`

GetDeploymentPolicyOk returns a tuple with the DeploymentPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentPolicy

`func (o *Environment) SetDeploymentPolicy(v string)`

SetDeploymentPolicy sets DeploymentPolicy field to given value.

### HasDeploymentPolicy

`func (o *Environment) HasDeploymentPolicy() bool`

HasDeploymentPolicy returns a boolean if a field has been set.

### GetLogVerbosity

`func (o *Environment) GetLogVerbosity() string`

GetLogVerbosity returns the LogVerbosity field if non-nil, zero value otherwise.

### GetLogVerbosityOk

`func (o *Environment) GetLogVerbosityOk() (*string, bool)`

GetLogVerbosityOk returns a tuple with the LogVerbosity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogVerbosity

`func (o *Environment) SetLogVerbosity(v string)`

SetLogVerbosity sets LogVerbosity field to given value.

### HasLogVerbosity

`func (o *Environment) HasLogVerbosity() bool`

HasLogVerbosity returns a boolean if a field has been set.

### GetRobotsPolicy

`func (o *Environment) GetRobotsPolicy() string`

GetRobotsPolicy returns the RobotsPolicy field if non-nil, zero value otherwise.

### GetRobotsPolicyOk

`func (o *Environment) GetRobotsPolicyOk() (*string, bool)`

GetRobotsPolicyOk returns a tuple with the RobotsPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRobotsPolicy

`func (o *Environment) SetRobotsPolicy(v string)`

SetRobotsPolicy sets RobotsPolicy field to given value.

### HasRobotsPolicy

`func (o *Environment) HasRobotsPolicy() bool`

HasRobotsPolicy returns a boolean if a field has been set.

### GetProtection

`func (o *Environment) GetProtection() EnvironmentProtection`

GetProtection returns the Protection field if non-nil, zero value otherwise.

### GetProtectionOk

`func (o *Environment) GetProtectionOk() (*EnvironmentProtection, bool)`

GetProtectionOk returns a tuple with the Protection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProtection

`func (o *Environment) SetProtection(v EnvironmentProtection)`

SetProtection sets Protection field to given value.

### HasProtection

`func (o *Environment) HasProtection() bool`

HasProtection returns a boolean if a field has been set.

### GetBranchTracking

`func (o *Environment) GetBranchTracking() EnvironmentBranchTracking`

GetBranchTracking returns the BranchTracking field if non-nil, zero value otherwise.

### GetBranchTrackingOk

`func (o *Environment) GetBranchTrackingOk() (*EnvironmentBranchTracking, bool)`

GetBranchTrackingOk returns a tuple with the BranchTracking field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranchTracking

`func (o *Environment) SetBranchTracking(v EnvironmentBranchTracking)`

SetBranchTracking sets BranchTracking field to given value.

### HasBranchTracking

`func (o *Environment) HasBranchTracking() bool`

HasBranchTracking returns a boolean if a field has been set.

### SetBranchTrackingNil

`func (o *Environment) SetBranchTrackingNil(b bool)`

 SetBranchTrackingNil sets the value for BranchTracking to be an explicit nil

### UnsetBranchTracking
`func (o *Environment) UnsetBranchTracking()`

UnsetBranchTracking ensures that no value is present for BranchTracking, not even an explicit nil
### GetVersionState

`func (o *Environment) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *Environment) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *Environment) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *Environment) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetProductVersion

`func (o *Environment) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *Environment) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *Environment) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.

### HasProductVersion

`func (o *Environment) HasProductVersion() bool`

HasProductVersion returns a boolean if a field has been set.

### GetClientId

`func (o *Environment) GetClientId() string`

GetClientId returns the ClientId field if non-nil, zero value otherwise.

### GetClientIdOk

`func (o *Environment) GetClientIdOk() (*string, bool)`

GetClientIdOk returns a tuple with the ClientId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientId

`func (o *Environment) SetClientId(v string)`

SetClientId sets ClientId field to given value.

### HasClientId

`func (o *Environment) HasClientId() bool`

HasClientId returns a boolean if a field has been set.

### GetCreatedAt

`func (o *Environment) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Environment) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Environment) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *Environment) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetLastModified

`func (o *Environment) GetLastModified() time.Time`

GetLastModified returns the LastModified field if non-nil, zero value otherwise.

### GetLastModifiedOk

`func (o *Environment) GetLastModifiedOk() (*time.Time, bool)`

GetLastModifiedOk returns a tuple with the LastModified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastModified

`func (o *Environment) SetLastModified(v time.Time)`

SetLastModified sets LastModified field to given value.

### HasLastModified

`func (o *Environment) HasLastModified() bool`

HasLastModified returns a boolean if a field has been set.

### SetLastModifiedNil

`func (o *Environment) SetLastModifiedNil(b bool)`

 SetLastModifiedNil sets the value for LastModified to be an explicit nil

### UnsetLastModified
`func (o *Environment) UnsetLastModified()`

UnsetLastModified ensures that no value is present for LastModified, not even an explicit nil
### GetCreatedBy

`func (o *Environment) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *Environment) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *Environment) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.

### HasCreatedBy

`func (o *Environment) HasCreatedBy() bool`

HasCreatedBy returns a boolean if a field has been set.

### SetCreatedByNil

`func (o *Environment) SetCreatedByNil(b bool)`

 SetCreatedByNil sets the value for CreatedBy to be an explicit nil

### UnsetCreatedBy
`func (o *Environment) UnsetCreatedBy()`

UnsetCreatedBy ensures that no value is present for CreatedBy, not even an explicit nil
### GetLastEditor

`func (o *Environment) GetLastEditor() string`

GetLastEditor returns the LastEditor field if non-nil, zero value otherwise.

### GetLastEditorOk

`func (o *Environment) GetLastEditorOk() (*string, bool)`

GetLastEditorOk returns a tuple with the LastEditor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEditor

`func (o *Environment) SetLastEditor(v string)`

SetLastEditor sets LastEditor field to given value.

### HasLastEditor

`func (o *Environment) HasLastEditor() bool`

HasLastEditor returns a boolean if a field has been set.

### SetLastEditorNil

`func (o *Environment) SetLastEditorNil(b bool)`

 SetLastEditorNil sets the value for LastEditor to be an explicit nil

### UnsetLastEditor
`func (o *Environment) UnsetLastEditor()`

UnsetLastEditor ensures that no value is present for LastEditor, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


