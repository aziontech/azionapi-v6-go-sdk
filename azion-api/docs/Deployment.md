# Deployment

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**VersionId** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **NullableString** |  | [optional] 
**BindingPolicy** | Pointer to **string** | * &#x60;STRICT&#x60; - STRICT * &#x60;FLEXIBLE&#x60; - FLEXIBLE | [optional] 
**DeploymentPolicy** | Pointer to **string** | * &#x60;single_version&#x60; - single_version * &#x60;versioned_urls&#x60; - versioned_urls | [optional] 
**StrategyDefaults** | Pointer to [**DeploymentStrategyDefaults**](DeploymentStrategyDefaults.md) |  | [optional] 
**VersionState** | Pointer to **string** | * &#x60;draft&#x60; - draft * &#x60;queued&#x60; - queued * &#x60;building&#x60; - building * &#x60;ready&#x60; - ready * &#x60;error&#x60; - error * &#x60;canceled&#x60; - canceled * &#x60;archiving&#x60; - archiving * &#x60;archived&#x60; - archived * &#x60;deleting&#x60; - deleting * &#x60;deleted&#x60; - deleted | [optional] 
**ProductVersion** | Pointer to **string** |  | [optional] 
**ClientId** | Pointer to **string** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**LastModified** | Pointer to **NullableTime** |  | [optional] 
**CreatedBy** | Pointer to **NullableString** |  | [optional] 
**LastEditor** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewDeployment

`func NewDeployment() *Deployment`

NewDeployment instantiates a new Deployment object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeploymentWithDefaults

`func NewDeploymentWithDefaults() *Deployment`

NewDeploymentWithDefaults instantiates a new Deployment object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Deployment) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Deployment) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Deployment) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *Deployment) HasId() bool`

HasId returns a boolean if a field has been set.

### GetVersionId

`func (o *Deployment) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *Deployment) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *Deployment) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *Deployment) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### GetName

`func (o *Deployment) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Deployment) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Deployment) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *Deployment) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *Deployment) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *Deployment) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *Deployment) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *Deployment) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *Deployment) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *Deployment) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetBindingPolicy

`func (o *Deployment) GetBindingPolicy() string`

GetBindingPolicy returns the BindingPolicy field if non-nil, zero value otherwise.

### GetBindingPolicyOk

`func (o *Deployment) GetBindingPolicyOk() (*string, bool)`

GetBindingPolicyOk returns a tuple with the BindingPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBindingPolicy

`func (o *Deployment) SetBindingPolicy(v string)`

SetBindingPolicy sets BindingPolicy field to given value.

### HasBindingPolicy

`func (o *Deployment) HasBindingPolicy() bool`

HasBindingPolicy returns a boolean if a field has been set.

### GetDeploymentPolicy

`func (o *Deployment) GetDeploymentPolicy() string`

GetDeploymentPolicy returns the DeploymentPolicy field if non-nil, zero value otherwise.

### GetDeploymentPolicyOk

`func (o *Deployment) GetDeploymentPolicyOk() (*string, bool)`

GetDeploymentPolicyOk returns a tuple with the DeploymentPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentPolicy

`func (o *Deployment) SetDeploymentPolicy(v string)`

SetDeploymentPolicy sets DeploymentPolicy field to given value.

### HasDeploymentPolicy

`func (o *Deployment) HasDeploymentPolicy() bool`

HasDeploymentPolicy returns a boolean if a field has been set.

### GetStrategyDefaults

`func (o *Deployment) GetStrategyDefaults() DeploymentStrategyDefaults`

GetStrategyDefaults returns the StrategyDefaults field if non-nil, zero value otherwise.

### GetStrategyDefaultsOk

`func (o *Deployment) GetStrategyDefaultsOk() (*DeploymentStrategyDefaults, bool)`

GetStrategyDefaultsOk returns a tuple with the StrategyDefaults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStrategyDefaults

`func (o *Deployment) SetStrategyDefaults(v DeploymentStrategyDefaults)`

SetStrategyDefaults sets StrategyDefaults field to given value.

### HasStrategyDefaults

`func (o *Deployment) HasStrategyDefaults() bool`

HasStrategyDefaults returns a boolean if a field has been set.

### GetVersionState

`func (o *Deployment) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *Deployment) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *Deployment) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *Deployment) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetProductVersion

`func (o *Deployment) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *Deployment) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *Deployment) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.

### HasProductVersion

`func (o *Deployment) HasProductVersion() bool`

HasProductVersion returns a boolean if a field has been set.

### GetClientId

`func (o *Deployment) GetClientId() string`

GetClientId returns the ClientId field if non-nil, zero value otherwise.

### GetClientIdOk

`func (o *Deployment) GetClientIdOk() (*string, bool)`

GetClientIdOk returns a tuple with the ClientId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientId

`func (o *Deployment) SetClientId(v string)`

SetClientId sets ClientId field to given value.

### HasClientId

`func (o *Deployment) HasClientId() bool`

HasClientId returns a boolean if a field has been set.

### GetCreatedAt

`func (o *Deployment) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Deployment) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Deployment) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *Deployment) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetLastModified

`func (o *Deployment) GetLastModified() time.Time`

GetLastModified returns the LastModified field if non-nil, zero value otherwise.

### GetLastModifiedOk

`func (o *Deployment) GetLastModifiedOk() (*time.Time, bool)`

GetLastModifiedOk returns a tuple with the LastModified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastModified

`func (o *Deployment) SetLastModified(v time.Time)`

SetLastModified sets LastModified field to given value.

### HasLastModified

`func (o *Deployment) HasLastModified() bool`

HasLastModified returns a boolean if a field has been set.

### SetLastModifiedNil

`func (o *Deployment) SetLastModifiedNil(b bool)`

 SetLastModifiedNil sets the value for LastModified to be an explicit nil

### UnsetLastModified
`func (o *Deployment) UnsetLastModified()`

UnsetLastModified ensures that no value is present for LastModified, not even an explicit nil
### GetCreatedBy

`func (o *Deployment) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *Deployment) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *Deployment) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.

### HasCreatedBy

`func (o *Deployment) HasCreatedBy() bool`

HasCreatedBy returns a boolean if a field has been set.

### SetCreatedByNil

`func (o *Deployment) SetCreatedByNil(b bool)`

 SetCreatedByNil sets the value for CreatedBy to be an explicit nil

### UnsetCreatedBy
`func (o *Deployment) UnsetCreatedBy()`

UnsetCreatedBy ensures that no value is present for CreatedBy, not even an explicit nil
### GetLastEditor

`func (o *Deployment) GetLastEditor() string`

GetLastEditor returns the LastEditor field if non-nil, zero value otherwise.

### GetLastEditorOk

`func (o *Deployment) GetLastEditorOk() (*string, bool)`

GetLastEditorOk returns a tuple with the LastEditor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEditor

`func (o *Deployment) SetLastEditor(v string)`

SetLastEditor sets LastEditor field to given value.

### HasLastEditor

`func (o *Deployment) HasLastEditor() bool`

HasLastEditor returns a boolean if a field has been set.

### SetLastEditorNil

`func (o *Deployment) SetLastEditorNil(b bool)`

 SetLastEditorNil sets the value for LastEditor to be an explicit nil

### UnsetLastEditor
`func (o *Deployment) UnsetLastEditor()`

UnsetLastEditor ensures that no value is present for LastEditor, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


