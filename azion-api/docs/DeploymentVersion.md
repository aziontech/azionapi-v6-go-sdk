# DeploymentVersion

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**VersionId** | Pointer to **string** | ID of the version metadata. | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **NullableString** |  | [optional] 
**BindingPolicy** | Pointer to **string** | * &#x60;STRICT&#x60; - STRICT * &#x60;FLEXIBLE&#x60; - FLEXIBLE | [optional] 
**DeploymentPolicy** | Pointer to **string** | * &#x60;single_version&#x60; - single_version * &#x60;versioned_urls&#x60; - versioned_urls | [optional] 
**StrategyDefaults** | Pointer to [**DeploymentStrategyDefaults**](DeploymentStrategyDefaults.md) |  | [optional] 
**VersionState** | Pointer to **string** | Current lifecycle state of the version.  * &#x60;draft&#x60; - draft * &#x60;queued&#x60; - queued * &#x60;building&#x60; - building * &#x60;ready&#x60; - ready * &#x60;error&#x60; - error * &#x60;canceled&#x60; - canceled * &#x60;archiving&#x60; - archiving * &#x60;archived&#x60; - archived * &#x60;deleting&#x60; - deleting * &#x60;deleted&#x60; - deleted | [optional] 
**ProductVersion** | Pointer to **NullableString** | Product version string. | [optional] 
**ClientId** | Pointer to **string** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** | When this version was created. | [optional] 
**LastModified** | Pointer to **NullableTime** |  | [optional] 
**CreatedBy** | Pointer to **NullableString** |  | [optional] 
**LastEditor** | Pointer to **NullableString** |  | [optional] 
**SourceVersionId** | Pointer to **NullableString** | ID of the source version if cloned. | [optional] 
**Snapshot** | Pointer to **map[string]interface{}** | JSON snapshot of the version data. | [optional] 
**ReadyAt** | Pointer to **NullableTime** | When this version became ready. | [optional] 
**BuildAt** | Pointer to **NullableTime** | When a build was triggered. | [optional] 
**BuildComment** | Pointer to **NullableString** | Comment provided when triggering the build. | [optional] 
**CancelAt** | Pointer to **NullableTime** | When a cancel was triggered. | [optional] 
**CancelComment** | Pointer to **NullableString** | Comment provided when cancelling the build. | [optional] 
**ArchivedAt** | Pointer to **NullableTime** | When this version was archived. | [optional] 
**ArchiveComment** | Pointer to **NullableString** | Comment provided when archiving. | [optional] 
**LastError** | Pointer to **map[string]interface{}** | Last build error details. | [optional] 
**TraceId** | Pointer to **NullableString** | Trace ID of the last outbox event of this version, null when the version never emitted one. | [optional] 

## Methods

### NewDeploymentVersion

`func NewDeploymentVersion() *DeploymentVersion`

NewDeploymentVersion instantiates a new DeploymentVersion object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeploymentVersionWithDefaults

`func NewDeploymentVersionWithDefaults() *DeploymentVersion`

NewDeploymentVersionWithDefaults instantiates a new DeploymentVersion object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersionId

`func (o *DeploymentVersion) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *DeploymentVersion) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *DeploymentVersion) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *DeploymentVersion) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### GetName

`func (o *DeploymentVersion) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *DeploymentVersion) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *DeploymentVersion) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *DeploymentVersion) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *DeploymentVersion) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *DeploymentVersion) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *DeploymentVersion) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *DeploymentVersion) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *DeploymentVersion) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *DeploymentVersion) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetBindingPolicy

`func (o *DeploymentVersion) GetBindingPolicy() string`

GetBindingPolicy returns the BindingPolicy field if non-nil, zero value otherwise.

### GetBindingPolicyOk

`func (o *DeploymentVersion) GetBindingPolicyOk() (*string, bool)`

GetBindingPolicyOk returns a tuple with the BindingPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBindingPolicy

`func (o *DeploymentVersion) SetBindingPolicy(v string)`

SetBindingPolicy sets BindingPolicy field to given value.

### HasBindingPolicy

`func (o *DeploymentVersion) HasBindingPolicy() bool`

HasBindingPolicy returns a boolean if a field has been set.

### GetDeploymentPolicy

`func (o *DeploymentVersion) GetDeploymentPolicy() string`

GetDeploymentPolicy returns the DeploymentPolicy field if non-nil, zero value otherwise.

### GetDeploymentPolicyOk

`func (o *DeploymentVersion) GetDeploymentPolicyOk() (*string, bool)`

GetDeploymentPolicyOk returns a tuple with the DeploymentPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentPolicy

`func (o *DeploymentVersion) SetDeploymentPolicy(v string)`

SetDeploymentPolicy sets DeploymentPolicy field to given value.

### HasDeploymentPolicy

`func (o *DeploymentVersion) HasDeploymentPolicy() bool`

HasDeploymentPolicy returns a boolean if a field has been set.

### GetStrategyDefaults

`func (o *DeploymentVersion) GetStrategyDefaults() DeploymentStrategyDefaults`

GetStrategyDefaults returns the StrategyDefaults field if non-nil, zero value otherwise.

### GetStrategyDefaultsOk

`func (o *DeploymentVersion) GetStrategyDefaultsOk() (*DeploymentStrategyDefaults, bool)`

GetStrategyDefaultsOk returns a tuple with the StrategyDefaults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStrategyDefaults

`func (o *DeploymentVersion) SetStrategyDefaults(v DeploymentStrategyDefaults)`

SetStrategyDefaults sets StrategyDefaults field to given value.

### HasStrategyDefaults

`func (o *DeploymentVersion) HasStrategyDefaults() bool`

HasStrategyDefaults returns a boolean if a field has been set.

### GetVersionState

`func (o *DeploymentVersion) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *DeploymentVersion) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *DeploymentVersion) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *DeploymentVersion) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetProductVersion

`func (o *DeploymentVersion) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *DeploymentVersion) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *DeploymentVersion) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.

### HasProductVersion

`func (o *DeploymentVersion) HasProductVersion() bool`

HasProductVersion returns a boolean if a field has been set.

### SetProductVersionNil

`func (o *DeploymentVersion) SetProductVersionNil(b bool)`

 SetProductVersionNil sets the value for ProductVersion to be an explicit nil

### UnsetProductVersion
`func (o *DeploymentVersion) UnsetProductVersion()`

UnsetProductVersion ensures that no value is present for ProductVersion, not even an explicit nil
### GetClientId

`func (o *DeploymentVersion) GetClientId() string`

GetClientId returns the ClientId field if non-nil, zero value otherwise.

### GetClientIdOk

`func (o *DeploymentVersion) GetClientIdOk() (*string, bool)`

GetClientIdOk returns a tuple with the ClientId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientId

`func (o *DeploymentVersion) SetClientId(v string)`

SetClientId sets ClientId field to given value.

### HasClientId

`func (o *DeploymentVersion) HasClientId() bool`

HasClientId returns a boolean if a field has been set.

### GetCreatedAt

`func (o *DeploymentVersion) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *DeploymentVersion) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *DeploymentVersion) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *DeploymentVersion) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetLastModified

`func (o *DeploymentVersion) GetLastModified() time.Time`

GetLastModified returns the LastModified field if non-nil, zero value otherwise.

### GetLastModifiedOk

`func (o *DeploymentVersion) GetLastModifiedOk() (*time.Time, bool)`

GetLastModifiedOk returns a tuple with the LastModified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastModified

`func (o *DeploymentVersion) SetLastModified(v time.Time)`

SetLastModified sets LastModified field to given value.

### HasLastModified

`func (o *DeploymentVersion) HasLastModified() bool`

HasLastModified returns a boolean if a field has been set.

### SetLastModifiedNil

`func (o *DeploymentVersion) SetLastModifiedNil(b bool)`

 SetLastModifiedNil sets the value for LastModified to be an explicit nil

### UnsetLastModified
`func (o *DeploymentVersion) UnsetLastModified()`

UnsetLastModified ensures that no value is present for LastModified, not even an explicit nil
### GetCreatedBy

`func (o *DeploymentVersion) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *DeploymentVersion) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *DeploymentVersion) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.

### HasCreatedBy

`func (o *DeploymentVersion) HasCreatedBy() bool`

HasCreatedBy returns a boolean if a field has been set.

### SetCreatedByNil

`func (o *DeploymentVersion) SetCreatedByNil(b bool)`

 SetCreatedByNil sets the value for CreatedBy to be an explicit nil

### UnsetCreatedBy
`func (o *DeploymentVersion) UnsetCreatedBy()`

UnsetCreatedBy ensures that no value is present for CreatedBy, not even an explicit nil
### GetLastEditor

`func (o *DeploymentVersion) GetLastEditor() string`

GetLastEditor returns the LastEditor field if non-nil, zero value otherwise.

### GetLastEditorOk

`func (o *DeploymentVersion) GetLastEditorOk() (*string, bool)`

GetLastEditorOk returns a tuple with the LastEditor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEditor

`func (o *DeploymentVersion) SetLastEditor(v string)`

SetLastEditor sets LastEditor field to given value.

### HasLastEditor

`func (o *DeploymentVersion) HasLastEditor() bool`

HasLastEditor returns a boolean if a field has been set.

### SetLastEditorNil

`func (o *DeploymentVersion) SetLastEditorNil(b bool)`

 SetLastEditorNil sets the value for LastEditor to be an explicit nil

### UnsetLastEditor
`func (o *DeploymentVersion) UnsetLastEditor()`

UnsetLastEditor ensures that no value is present for LastEditor, not even an explicit nil
### GetSourceVersionId

`func (o *DeploymentVersion) GetSourceVersionId() string`

GetSourceVersionId returns the SourceVersionId field if non-nil, zero value otherwise.

### GetSourceVersionIdOk

`func (o *DeploymentVersion) GetSourceVersionIdOk() (*string, bool)`

GetSourceVersionIdOk returns a tuple with the SourceVersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceVersionId

`func (o *DeploymentVersion) SetSourceVersionId(v string)`

SetSourceVersionId sets SourceVersionId field to given value.

### HasSourceVersionId

`func (o *DeploymentVersion) HasSourceVersionId() bool`

HasSourceVersionId returns a boolean if a field has been set.

### SetSourceVersionIdNil

`func (o *DeploymentVersion) SetSourceVersionIdNil(b bool)`

 SetSourceVersionIdNil sets the value for SourceVersionId to be an explicit nil

### UnsetSourceVersionId
`func (o *DeploymentVersion) UnsetSourceVersionId()`

UnsetSourceVersionId ensures that no value is present for SourceVersionId, not even an explicit nil
### GetSnapshot

`func (o *DeploymentVersion) GetSnapshot() map[string]interface{}`

GetSnapshot returns the Snapshot field if non-nil, zero value otherwise.

### GetSnapshotOk

`func (o *DeploymentVersion) GetSnapshotOk() (*map[string]interface{}, bool)`

GetSnapshotOk returns a tuple with the Snapshot field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnapshot

`func (o *DeploymentVersion) SetSnapshot(v map[string]interface{})`

SetSnapshot sets Snapshot field to given value.

### HasSnapshot

`func (o *DeploymentVersion) HasSnapshot() bool`

HasSnapshot returns a boolean if a field has been set.

### SetSnapshotNil

`func (o *DeploymentVersion) SetSnapshotNil(b bool)`

 SetSnapshotNil sets the value for Snapshot to be an explicit nil

### UnsetSnapshot
`func (o *DeploymentVersion) UnsetSnapshot()`

UnsetSnapshot ensures that no value is present for Snapshot, not even an explicit nil
### GetReadyAt

`func (o *DeploymentVersion) GetReadyAt() time.Time`

GetReadyAt returns the ReadyAt field if non-nil, zero value otherwise.

### GetReadyAtOk

`func (o *DeploymentVersion) GetReadyAtOk() (*time.Time, bool)`

GetReadyAtOk returns a tuple with the ReadyAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadyAt

`func (o *DeploymentVersion) SetReadyAt(v time.Time)`

SetReadyAt sets ReadyAt field to given value.

### HasReadyAt

`func (o *DeploymentVersion) HasReadyAt() bool`

HasReadyAt returns a boolean if a field has been set.

### SetReadyAtNil

`func (o *DeploymentVersion) SetReadyAtNil(b bool)`

 SetReadyAtNil sets the value for ReadyAt to be an explicit nil

### UnsetReadyAt
`func (o *DeploymentVersion) UnsetReadyAt()`

UnsetReadyAt ensures that no value is present for ReadyAt, not even an explicit nil
### GetBuildAt

`func (o *DeploymentVersion) GetBuildAt() time.Time`

GetBuildAt returns the BuildAt field if non-nil, zero value otherwise.

### GetBuildAtOk

`func (o *DeploymentVersion) GetBuildAtOk() (*time.Time, bool)`

GetBuildAtOk returns a tuple with the BuildAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildAt

`func (o *DeploymentVersion) SetBuildAt(v time.Time)`

SetBuildAt sets BuildAt field to given value.

### HasBuildAt

`func (o *DeploymentVersion) HasBuildAt() bool`

HasBuildAt returns a boolean if a field has been set.

### SetBuildAtNil

`func (o *DeploymentVersion) SetBuildAtNil(b bool)`

 SetBuildAtNil sets the value for BuildAt to be an explicit nil

### UnsetBuildAt
`func (o *DeploymentVersion) UnsetBuildAt()`

UnsetBuildAt ensures that no value is present for BuildAt, not even an explicit nil
### GetBuildComment

`func (o *DeploymentVersion) GetBuildComment() string`

GetBuildComment returns the BuildComment field if non-nil, zero value otherwise.

### GetBuildCommentOk

`func (o *DeploymentVersion) GetBuildCommentOk() (*string, bool)`

GetBuildCommentOk returns a tuple with the BuildComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildComment

`func (o *DeploymentVersion) SetBuildComment(v string)`

SetBuildComment sets BuildComment field to given value.

### HasBuildComment

`func (o *DeploymentVersion) HasBuildComment() bool`

HasBuildComment returns a boolean if a field has been set.

### SetBuildCommentNil

`func (o *DeploymentVersion) SetBuildCommentNil(b bool)`

 SetBuildCommentNil sets the value for BuildComment to be an explicit nil

### UnsetBuildComment
`func (o *DeploymentVersion) UnsetBuildComment()`

UnsetBuildComment ensures that no value is present for BuildComment, not even an explicit nil
### GetCancelAt

`func (o *DeploymentVersion) GetCancelAt() time.Time`

GetCancelAt returns the CancelAt field if non-nil, zero value otherwise.

### GetCancelAtOk

`func (o *DeploymentVersion) GetCancelAtOk() (*time.Time, bool)`

GetCancelAtOk returns a tuple with the CancelAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelAt

`func (o *DeploymentVersion) SetCancelAt(v time.Time)`

SetCancelAt sets CancelAt field to given value.

### HasCancelAt

`func (o *DeploymentVersion) HasCancelAt() bool`

HasCancelAt returns a boolean if a field has been set.

### SetCancelAtNil

`func (o *DeploymentVersion) SetCancelAtNil(b bool)`

 SetCancelAtNil sets the value for CancelAt to be an explicit nil

### UnsetCancelAt
`func (o *DeploymentVersion) UnsetCancelAt()`

UnsetCancelAt ensures that no value is present for CancelAt, not even an explicit nil
### GetCancelComment

`func (o *DeploymentVersion) GetCancelComment() string`

GetCancelComment returns the CancelComment field if non-nil, zero value otherwise.

### GetCancelCommentOk

`func (o *DeploymentVersion) GetCancelCommentOk() (*string, bool)`

GetCancelCommentOk returns a tuple with the CancelComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelComment

`func (o *DeploymentVersion) SetCancelComment(v string)`

SetCancelComment sets CancelComment field to given value.

### HasCancelComment

`func (o *DeploymentVersion) HasCancelComment() bool`

HasCancelComment returns a boolean if a field has been set.

### SetCancelCommentNil

`func (o *DeploymentVersion) SetCancelCommentNil(b bool)`

 SetCancelCommentNil sets the value for CancelComment to be an explicit nil

### UnsetCancelComment
`func (o *DeploymentVersion) UnsetCancelComment()`

UnsetCancelComment ensures that no value is present for CancelComment, not even an explicit nil
### GetArchivedAt

`func (o *DeploymentVersion) GetArchivedAt() time.Time`

GetArchivedAt returns the ArchivedAt field if non-nil, zero value otherwise.

### GetArchivedAtOk

`func (o *DeploymentVersion) GetArchivedAtOk() (*time.Time, bool)`

GetArchivedAtOk returns a tuple with the ArchivedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchivedAt

`func (o *DeploymentVersion) SetArchivedAt(v time.Time)`

SetArchivedAt sets ArchivedAt field to given value.

### HasArchivedAt

`func (o *DeploymentVersion) HasArchivedAt() bool`

HasArchivedAt returns a boolean if a field has been set.

### SetArchivedAtNil

`func (o *DeploymentVersion) SetArchivedAtNil(b bool)`

 SetArchivedAtNil sets the value for ArchivedAt to be an explicit nil

### UnsetArchivedAt
`func (o *DeploymentVersion) UnsetArchivedAt()`

UnsetArchivedAt ensures that no value is present for ArchivedAt, not even an explicit nil
### GetArchiveComment

`func (o *DeploymentVersion) GetArchiveComment() string`

GetArchiveComment returns the ArchiveComment field if non-nil, zero value otherwise.

### GetArchiveCommentOk

`func (o *DeploymentVersion) GetArchiveCommentOk() (*string, bool)`

GetArchiveCommentOk returns a tuple with the ArchiveComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchiveComment

`func (o *DeploymentVersion) SetArchiveComment(v string)`

SetArchiveComment sets ArchiveComment field to given value.

### HasArchiveComment

`func (o *DeploymentVersion) HasArchiveComment() bool`

HasArchiveComment returns a boolean if a field has been set.

### SetArchiveCommentNil

`func (o *DeploymentVersion) SetArchiveCommentNil(b bool)`

 SetArchiveCommentNil sets the value for ArchiveComment to be an explicit nil

### UnsetArchiveComment
`func (o *DeploymentVersion) UnsetArchiveComment()`

UnsetArchiveComment ensures that no value is present for ArchiveComment, not even an explicit nil
### GetLastError

`func (o *DeploymentVersion) GetLastError() map[string]interface{}`

GetLastError returns the LastError field if non-nil, zero value otherwise.

### GetLastErrorOk

`func (o *DeploymentVersion) GetLastErrorOk() (*map[string]interface{}, bool)`

GetLastErrorOk returns a tuple with the LastError field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastError

`func (o *DeploymentVersion) SetLastError(v map[string]interface{})`

SetLastError sets LastError field to given value.

### HasLastError

`func (o *DeploymentVersion) HasLastError() bool`

HasLastError returns a boolean if a field has been set.

### SetLastErrorNil

`func (o *DeploymentVersion) SetLastErrorNil(b bool)`

 SetLastErrorNil sets the value for LastError to be an explicit nil

### UnsetLastError
`func (o *DeploymentVersion) UnsetLastError()`

UnsetLastError ensures that no value is present for LastError, not even an explicit nil
### GetTraceId

`func (o *DeploymentVersion) GetTraceId() string`

GetTraceId returns the TraceId field if non-nil, zero value otherwise.

### GetTraceIdOk

`func (o *DeploymentVersion) GetTraceIdOk() (*string, bool)`

GetTraceIdOk returns a tuple with the TraceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraceId

`func (o *DeploymentVersion) SetTraceId(v string)`

SetTraceId sets TraceId field to given value.

### HasTraceId

`func (o *DeploymentVersion) HasTraceId() bool`

HasTraceId returns a boolean if a field has been set.

### SetTraceIdNil

`func (o *DeploymentVersion) SetTraceIdNil(b bool)`

 SetTraceIdNil sets the value for TraceId to be an explicit nil

### UnsetTraceId
`func (o *DeploymentVersion) UnsetTraceId()`

UnsetTraceId ensures that no value is present for TraceId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


