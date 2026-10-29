# AccountRelease

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**DeploymentId** | Pointer to **string** |  | [optional] 
**Resources** | Pointer to [**[]AccountReleaseResourcesInner**](AccountReleaseResourcesInner.md) |  | [optional] 
**TrafficRole** | Pointer to **string** | * &#x60;ACTIVE&#x60; - ACTIVE * &#x60;CANDIDATE&#x60; - CANDIDATE * &#x60;VALID_URL&#x60; - VALID_URL * &#x60;INACTIVE&#x60; - INACTIVE | [optional] 
**Origin** | Pointer to [**AccountReleaseOrigin**](AccountReleaseOrigin.md) |  | [optional] 
**State** | Pointer to **string** | * &#x60;draft&#x60; - draft * &#x60;queued&#x60; - queued * &#x60;building&#x60; - building * &#x60;ready&#x60; - ready * &#x60;error&#x60; - error * &#x60;canceled&#x60; - canceled * &#x60;archiving&#x60; - archiving * &#x60;archived&#x60; - archived * &#x60;deleting&#x60; - deleting * &#x60;deleted&#x60; - deleted | [optional] 
**ClientId** | Pointer to **string** |  | [optional] 
**ProductVersion** | Pointer to **string** |  | [optional] 
**CreatedBy** | Pointer to **NullableString** |  | [optional] 
**LastEditor** | Pointer to **NullableString** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**LastModified** | Pointer to **NullableTime** |  | [optional] 
**ReadyAt** | Pointer to **NullableTime** |  | [optional] 
**TraceId** | Pointer to **string** |  | [optional] 
**DeploymentName** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewAccountRelease

`func NewAccountRelease() *AccountRelease`

NewAccountRelease instantiates a new AccountRelease object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAccountReleaseWithDefaults

`func NewAccountReleaseWithDefaults() *AccountRelease`

NewAccountReleaseWithDefaults instantiates a new AccountRelease object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *AccountRelease) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AccountRelease) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AccountRelease) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *AccountRelease) HasId() bool`

HasId returns a boolean if a field has been set.

### GetDeploymentId

`func (o *AccountRelease) GetDeploymentId() string`

GetDeploymentId returns the DeploymentId field if non-nil, zero value otherwise.

### GetDeploymentIdOk

`func (o *AccountRelease) GetDeploymentIdOk() (*string, bool)`

GetDeploymentIdOk returns a tuple with the DeploymentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentId

`func (o *AccountRelease) SetDeploymentId(v string)`

SetDeploymentId sets DeploymentId field to given value.

### HasDeploymentId

`func (o *AccountRelease) HasDeploymentId() bool`

HasDeploymentId returns a boolean if a field has been set.

### GetResources

`func (o *AccountRelease) GetResources() []AccountReleaseResourcesInner`

GetResources returns the Resources field if non-nil, zero value otherwise.

### GetResourcesOk

`func (o *AccountRelease) GetResourcesOk() (*[]AccountReleaseResourcesInner, bool)`

GetResourcesOk returns a tuple with the Resources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResources

`func (o *AccountRelease) SetResources(v []AccountReleaseResourcesInner)`

SetResources sets Resources field to given value.

### HasResources

`func (o *AccountRelease) HasResources() bool`

HasResources returns a boolean if a field has been set.

### GetTrafficRole

`func (o *AccountRelease) GetTrafficRole() string`

GetTrafficRole returns the TrafficRole field if non-nil, zero value otherwise.

### GetTrafficRoleOk

`func (o *AccountRelease) GetTrafficRoleOk() (*string, bool)`

GetTrafficRoleOk returns a tuple with the TrafficRole field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrafficRole

`func (o *AccountRelease) SetTrafficRole(v string)`

SetTrafficRole sets TrafficRole field to given value.

### HasTrafficRole

`func (o *AccountRelease) HasTrafficRole() bool`

HasTrafficRole returns a boolean if a field has been set.

### GetOrigin

`func (o *AccountRelease) GetOrigin() AccountReleaseOrigin`

GetOrigin returns the Origin field if non-nil, zero value otherwise.

### GetOriginOk

`func (o *AccountRelease) GetOriginOk() (*AccountReleaseOrigin, bool)`

GetOriginOk returns a tuple with the Origin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrigin

`func (o *AccountRelease) SetOrigin(v AccountReleaseOrigin)`

SetOrigin sets Origin field to given value.

### HasOrigin

`func (o *AccountRelease) HasOrigin() bool`

HasOrigin returns a boolean if a field has been set.

### GetState

`func (o *AccountRelease) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *AccountRelease) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *AccountRelease) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *AccountRelease) HasState() bool`

HasState returns a boolean if a field has been set.

### GetClientId

`func (o *AccountRelease) GetClientId() string`

GetClientId returns the ClientId field if non-nil, zero value otherwise.

### GetClientIdOk

`func (o *AccountRelease) GetClientIdOk() (*string, bool)`

GetClientIdOk returns a tuple with the ClientId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientId

`func (o *AccountRelease) SetClientId(v string)`

SetClientId sets ClientId field to given value.

### HasClientId

`func (o *AccountRelease) HasClientId() bool`

HasClientId returns a boolean if a field has been set.

### GetProductVersion

`func (o *AccountRelease) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *AccountRelease) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *AccountRelease) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.

### HasProductVersion

`func (o *AccountRelease) HasProductVersion() bool`

HasProductVersion returns a boolean if a field has been set.

### GetCreatedBy

`func (o *AccountRelease) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *AccountRelease) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *AccountRelease) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.

### HasCreatedBy

`func (o *AccountRelease) HasCreatedBy() bool`

HasCreatedBy returns a boolean if a field has been set.

### SetCreatedByNil

`func (o *AccountRelease) SetCreatedByNil(b bool)`

 SetCreatedByNil sets the value for CreatedBy to be an explicit nil

### UnsetCreatedBy
`func (o *AccountRelease) UnsetCreatedBy()`

UnsetCreatedBy ensures that no value is present for CreatedBy, not even an explicit nil
### GetLastEditor

`func (o *AccountRelease) GetLastEditor() string`

GetLastEditor returns the LastEditor field if non-nil, zero value otherwise.

### GetLastEditorOk

`func (o *AccountRelease) GetLastEditorOk() (*string, bool)`

GetLastEditorOk returns a tuple with the LastEditor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEditor

`func (o *AccountRelease) SetLastEditor(v string)`

SetLastEditor sets LastEditor field to given value.

### HasLastEditor

`func (o *AccountRelease) HasLastEditor() bool`

HasLastEditor returns a boolean if a field has been set.

### SetLastEditorNil

`func (o *AccountRelease) SetLastEditorNil(b bool)`

 SetLastEditorNil sets the value for LastEditor to be an explicit nil

### UnsetLastEditor
`func (o *AccountRelease) UnsetLastEditor()`

UnsetLastEditor ensures that no value is present for LastEditor, not even an explicit nil
### GetCreatedAt

`func (o *AccountRelease) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *AccountRelease) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *AccountRelease) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *AccountRelease) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetLastModified

`func (o *AccountRelease) GetLastModified() time.Time`

GetLastModified returns the LastModified field if non-nil, zero value otherwise.

### GetLastModifiedOk

`func (o *AccountRelease) GetLastModifiedOk() (*time.Time, bool)`

GetLastModifiedOk returns a tuple with the LastModified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastModified

`func (o *AccountRelease) SetLastModified(v time.Time)`

SetLastModified sets LastModified field to given value.

### HasLastModified

`func (o *AccountRelease) HasLastModified() bool`

HasLastModified returns a boolean if a field has been set.

### SetLastModifiedNil

`func (o *AccountRelease) SetLastModifiedNil(b bool)`

 SetLastModifiedNil sets the value for LastModified to be an explicit nil

### UnsetLastModified
`func (o *AccountRelease) UnsetLastModified()`

UnsetLastModified ensures that no value is present for LastModified, not even an explicit nil
### GetReadyAt

`func (o *AccountRelease) GetReadyAt() time.Time`

GetReadyAt returns the ReadyAt field if non-nil, zero value otherwise.

### GetReadyAtOk

`func (o *AccountRelease) GetReadyAtOk() (*time.Time, bool)`

GetReadyAtOk returns a tuple with the ReadyAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadyAt

`func (o *AccountRelease) SetReadyAt(v time.Time)`

SetReadyAt sets ReadyAt field to given value.

### HasReadyAt

`func (o *AccountRelease) HasReadyAt() bool`

HasReadyAt returns a boolean if a field has been set.

### SetReadyAtNil

`func (o *AccountRelease) SetReadyAtNil(b bool)`

 SetReadyAtNil sets the value for ReadyAt to be an explicit nil

### UnsetReadyAt
`func (o *AccountRelease) UnsetReadyAt()`

UnsetReadyAt ensures that no value is present for ReadyAt, not even an explicit nil
### GetTraceId

`func (o *AccountRelease) GetTraceId() string`

GetTraceId returns the TraceId field if non-nil, zero value otherwise.

### GetTraceIdOk

`func (o *AccountRelease) GetTraceIdOk() (*string, bool)`

GetTraceIdOk returns a tuple with the TraceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraceId

`func (o *AccountRelease) SetTraceId(v string)`

SetTraceId sets TraceId field to given value.

### HasTraceId

`func (o *AccountRelease) HasTraceId() bool`

HasTraceId returns a boolean if a field has been set.

### GetDeploymentName

`func (o *AccountRelease) GetDeploymentName() string`

GetDeploymentName returns the DeploymentName field if non-nil, zero value otherwise.

### GetDeploymentNameOk

`func (o *AccountRelease) GetDeploymentNameOk() (*string, bool)`

GetDeploymentNameOk returns a tuple with the DeploymentName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentName

`func (o *AccountRelease) SetDeploymentName(v string)`

SetDeploymentName sets DeploymentName field to given value.

### HasDeploymentName

`func (o *AccountRelease) HasDeploymentName() bool`

HasDeploymentName returns a boolean if a field has been set.

### SetDeploymentNameNil

`func (o *AccountRelease) SetDeploymentNameNil(b bool)`

 SetDeploymentNameNil sets the value for DeploymentName to be an explicit nil

### UnsetDeploymentName
`func (o *AccountRelease) UnsetDeploymentName()`

UnsetDeploymentName ensures that no value is present for DeploymentName, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


