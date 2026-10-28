# Release

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

## Methods

### NewRelease

`func NewRelease() *Release`

NewRelease instantiates a new Release object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReleaseWithDefaults

`func NewReleaseWithDefaults() *Release`

NewReleaseWithDefaults instantiates a new Release object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Release) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Release) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Release) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *Release) HasId() bool`

HasId returns a boolean if a field has been set.

### GetDeploymentId

`func (o *Release) GetDeploymentId() string`

GetDeploymentId returns the DeploymentId field if non-nil, zero value otherwise.

### GetDeploymentIdOk

`func (o *Release) GetDeploymentIdOk() (*string, bool)`

GetDeploymentIdOk returns a tuple with the DeploymentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentId

`func (o *Release) SetDeploymentId(v string)`

SetDeploymentId sets DeploymentId field to given value.

### HasDeploymentId

`func (o *Release) HasDeploymentId() bool`

HasDeploymentId returns a boolean if a field has been set.

### GetResources

`func (o *Release) GetResources() []AccountReleaseResourcesInner`

GetResources returns the Resources field if non-nil, zero value otherwise.

### GetResourcesOk

`func (o *Release) GetResourcesOk() (*[]AccountReleaseResourcesInner, bool)`

GetResourcesOk returns a tuple with the Resources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResources

`func (o *Release) SetResources(v []AccountReleaseResourcesInner)`

SetResources sets Resources field to given value.

### HasResources

`func (o *Release) HasResources() bool`

HasResources returns a boolean if a field has been set.

### GetTrafficRole

`func (o *Release) GetTrafficRole() string`

GetTrafficRole returns the TrafficRole field if non-nil, zero value otherwise.

### GetTrafficRoleOk

`func (o *Release) GetTrafficRoleOk() (*string, bool)`

GetTrafficRoleOk returns a tuple with the TrafficRole field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrafficRole

`func (o *Release) SetTrafficRole(v string)`

SetTrafficRole sets TrafficRole field to given value.

### HasTrafficRole

`func (o *Release) HasTrafficRole() bool`

HasTrafficRole returns a boolean if a field has been set.

### GetOrigin

`func (o *Release) GetOrigin() AccountReleaseOrigin`

GetOrigin returns the Origin field if non-nil, zero value otherwise.

### GetOriginOk

`func (o *Release) GetOriginOk() (*AccountReleaseOrigin, bool)`

GetOriginOk returns a tuple with the Origin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrigin

`func (o *Release) SetOrigin(v AccountReleaseOrigin)`

SetOrigin sets Origin field to given value.

### HasOrigin

`func (o *Release) HasOrigin() bool`

HasOrigin returns a boolean if a field has been set.

### GetState

`func (o *Release) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *Release) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *Release) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *Release) HasState() bool`

HasState returns a boolean if a field has been set.

### GetClientId

`func (o *Release) GetClientId() string`

GetClientId returns the ClientId field if non-nil, zero value otherwise.

### GetClientIdOk

`func (o *Release) GetClientIdOk() (*string, bool)`

GetClientIdOk returns a tuple with the ClientId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientId

`func (o *Release) SetClientId(v string)`

SetClientId sets ClientId field to given value.

### HasClientId

`func (o *Release) HasClientId() bool`

HasClientId returns a boolean if a field has been set.

### GetProductVersion

`func (o *Release) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *Release) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *Release) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.

### HasProductVersion

`func (o *Release) HasProductVersion() bool`

HasProductVersion returns a boolean if a field has been set.

### GetCreatedBy

`func (o *Release) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *Release) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *Release) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.

### HasCreatedBy

`func (o *Release) HasCreatedBy() bool`

HasCreatedBy returns a boolean if a field has been set.

### SetCreatedByNil

`func (o *Release) SetCreatedByNil(b bool)`

 SetCreatedByNil sets the value for CreatedBy to be an explicit nil

### UnsetCreatedBy
`func (o *Release) UnsetCreatedBy()`

UnsetCreatedBy ensures that no value is present for CreatedBy, not even an explicit nil
### GetLastEditor

`func (o *Release) GetLastEditor() string`

GetLastEditor returns the LastEditor field if non-nil, zero value otherwise.

### GetLastEditorOk

`func (o *Release) GetLastEditorOk() (*string, bool)`

GetLastEditorOk returns a tuple with the LastEditor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEditor

`func (o *Release) SetLastEditor(v string)`

SetLastEditor sets LastEditor field to given value.

### HasLastEditor

`func (o *Release) HasLastEditor() bool`

HasLastEditor returns a boolean if a field has been set.

### SetLastEditorNil

`func (o *Release) SetLastEditorNil(b bool)`

 SetLastEditorNil sets the value for LastEditor to be an explicit nil

### UnsetLastEditor
`func (o *Release) UnsetLastEditor()`

UnsetLastEditor ensures that no value is present for LastEditor, not even an explicit nil
### GetCreatedAt

`func (o *Release) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Release) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Release) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *Release) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetLastModified

`func (o *Release) GetLastModified() time.Time`

GetLastModified returns the LastModified field if non-nil, zero value otherwise.

### GetLastModifiedOk

`func (o *Release) GetLastModifiedOk() (*time.Time, bool)`

GetLastModifiedOk returns a tuple with the LastModified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastModified

`func (o *Release) SetLastModified(v time.Time)`

SetLastModified sets LastModified field to given value.

### HasLastModified

`func (o *Release) HasLastModified() bool`

HasLastModified returns a boolean if a field has been set.

### SetLastModifiedNil

`func (o *Release) SetLastModifiedNil(b bool)`

 SetLastModifiedNil sets the value for LastModified to be an explicit nil

### UnsetLastModified
`func (o *Release) UnsetLastModified()`

UnsetLastModified ensures that no value is present for LastModified, not even an explicit nil
### GetReadyAt

`func (o *Release) GetReadyAt() time.Time`

GetReadyAt returns the ReadyAt field if non-nil, zero value otherwise.

### GetReadyAtOk

`func (o *Release) GetReadyAtOk() (*time.Time, bool)`

GetReadyAtOk returns a tuple with the ReadyAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadyAt

`func (o *Release) SetReadyAt(v time.Time)`

SetReadyAt sets ReadyAt field to given value.

### HasReadyAt

`func (o *Release) HasReadyAt() bool`

HasReadyAt returns a boolean if a field has been set.

### SetReadyAtNil

`func (o *Release) SetReadyAtNil(b bool)`

 SetReadyAtNil sets the value for ReadyAt to be an explicit nil

### UnsetReadyAt
`func (o *Release) UnsetReadyAt()`

UnsetReadyAt ensures that no value is present for ReadyAt, not even an explicit nil
### GetTraceId

`func (o *Release) GetTraceId() string`

GetTraceId returns the TraceId field if non-nil, zero value otherwise.

### GetTraceIdOk

`func (o *Release) GetTraceIdOk() (*string, bool)`

GetTraceIdOk returns a tuple with the TraceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraceId

`func (o *Release) SetTraceId(v string)`

SetTraceId sets TraceId field to given value.

### HasTraceId

`func (o *Release) HasTraceId() bool`

HasTraceId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


