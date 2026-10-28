# DeploymentVersionMeta

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**VersionId** | Pointer to **string** | ID of the version metadata. | [optional] 
**VersionState** | Pointer to **string** | Current lifecycle state of the version.  * &#x60;draft&#x60; - draft * &#x60;queued&#x60; - queued * &#x60;building&#x60; - building * &#x60;ready&#x60; - ready * &#x60;error&#x60; - error * &#x60;canceled&#x60; - canceled * &#x60;archiving&#x60; - archiving * &#x60;archived&#x60; - archived * &#x60;deleting&#x60; - deleting * &#x60;deleted&#x60; - deleted | [optional] 
**ProductVersion** | Pointer to **NullableString** | Product version string. | [optional] 
**SourceVersionId** | Pointer to **NullableString** | ID of the source version if cloned. | [optional] 
**Snapshot** | Pointer to **map[string]interface{}** | JSON snapshot of the version data. | [optional] 
**CreatedAt** | Pointer to **time.Time** | When this version was created. | [optional] 
**ReadyAt** | Pointer to **NullableTime** | When this version became ready. | [optional] 
**Description** | Pointer to **NullableString** | Version description, sent only when the adapter supplies one. | [optional] 
**BuildAt** | Pointer to **NullableTime** | When a build was triggered. | [optional] 
**BuildComment** | Pointer to **NullableString** | Comment provided when triggering the build. | [optional] 
**CancelAt** | Pointer to **NullableTime** | When a cancel was triggered. | [optional] 
**CancelComment** | Pointer to **NullableString** | Comment provided when cancelling the build. | [optional] 
**ArchivedAt** | Pointer to **NullableTime** | When this version was archived. | [optional] 
**ArchiveComment** | Pointer to **NullableString** | Comment provided when archiving. | [optional] 
**LastError** | Pointer to **map[string]interface{}** | Last build error details. | [optional] 
**TraceId** | Pointer to **NullableString** | Trace ID of the last outbox event of this version, null when the version never emitted one. | [optional] 

## Methods

### NewDeploymentVersionMeta

`func NewDeploymentVersionMeta() *DeploymentVersionMeta`

NewDeploymentVersionMeta instantiates a new DeploymentVersionMeta object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeploymentVersionMetaWithDefaults

`func NewDeploymentVersionMetaWithDefaults() *DeploymentVersionMeta`

NewDeploymentVersionMetaWithDefaults instantiates a new DeploymentVersionMeta object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersionId

`func (o *DeploymentVersionMeta) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *DeploymentVersionMeta) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *DeploymentVersionMeta) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *DeploymentVersionMeta) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### GetVersionState

`func (o *DeploymentVersionMeta) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *DeploymentVersionMeta) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *DeploymentVersionMeta) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *DeploymentVersionMeta) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetProductVersion

`func (o *DeploymentVersionMeta) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *DeploymentVersionMeta) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *DeploymentVersionMeta) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.

### HasProductVersion

`func (o *DeploymentVersionMeta) HasProductVersion() bool`

HasProductVersion returns a boolean if a field has been set.

### SetProductVersionNil

`func (o *DeploymentVersionMeta) SetProductVersionNil(b bool)`

 SetProductVersionNil sets the value for ProductVersion to be an explicit nil

### UnsetProductVersion
`func (o *DeploymentVersionMeta) UnsetProductVersion()`

UnsetProductVersion ensures that no value is present for ProductVersion, not even an explicit nil
### GetSourceVersionId

`func (o *DeploymentVersionMeta) GetSourceVersionId() string`

GetSourceVersionId returns the SourceVersionId field if non-nil, zero value otherwise.

### GetSourceVersionIdOk

`func (o *DeploymentVersionMeta) GetSourceVersionIdOk() (*string, bool)`

GetSourceVersionIdOk returns a tuple with the SourceVersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceVersionId

`func (o *DeploymentVersionMeta) SetSourceVersionId(v string)`

SetSourceVersionId sets SourceVersionId field to given value.

### HasSourceVersionId

`func (o *DeploymentVersionMeta) HasSourceVersionId() bool`

HasSourceVersionId returns a boolean if a field has been set.

### SetSourceVersionIdNil

`func (o *DeploymentVersionMeta) SetSourceVersionIdNil(b bool)`

 SetSourceVersionIdNil sets the value for SourceVersionId to be an explicit nil

### UnsetSourceVersionId
`func (o *DeploymentVersionMeta) UnsetSourceVersionId()`

UnsetSourceVersionId ensures that no value is present for SourceVersionId, not even an explicit nil
### GetSnapshot

`func (o *DeploymentVersionMeta) GetSnapshot() map[string]interface{}`

GetSnapshot returns the Snapshot field if non-nil, zero value otherwise.

### GetSnapshotOk

`func (o *DeploymentVersionMeta) GetSnapshotOk() (*map[string]interface{}, bool)`

GetSnapshotOk returns a tuple with the Snapshot field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnapshot

`func (o *DeploymentVersionMeta) SetSnapshot(v map[string]interface{})`

SetSnapshot sets Snapshot field to given value.

### HasSnapshot

`func (o *DeploymentVersionMeta) HasSnapshot() bool`

HasSnapshot returns a boolean if a field has been set.

### SetSnapshotNil

`func (o *DeploymentVersionMeta) SetSnapshotNil(b bool)`

 SetSnapshotNil sets the value for Snapshot to be an explicit nil

### UnsetSnapshot
`func (o *DeploymentVersionMeta) UnsetSnapshot()`

UnsetSnapshot ensures that no value is present for Snapshot, not even an explicit nil
### GetCreatedAt

`func (o *DeploymentVersionMeta) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *DeploymentVersionMeta) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *DeploymentVersionMeta) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *DeploymentVersionMeta) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetReadyAt

`func (o *DeploymentVersionMeta) GetReadyAt() time.Time`

GetReadyAt returns the ReadyAt field if non-nil, zero value otherwise.

### GetReadyAtOk

`func (o *DeploymentVersionMeta) GetReadyAtOk() (*time.Time, bool)`

GetReadyAtOk returns a tuple with the ReadyAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadyAt

`func (o *DeploymentVersionMeta) SetReadyAt(v time.Time)`

SetReadyAt sets ReadyAt field to given value.

### HasReadyAt

`func (o *DeploymentVersionMeta) HasReadyAt() bool`

HasReadyAt returns a boolean if a field has been set.

### SetReadyAtNil

`func (o *DeploymentVersionMeta) SetReadyAtNil(b bool)`

 SetReadyAtNil sets the value for ReadyAt to be an explicit nil

### UnsetReadyAt
`func (o *DeploymentVersionMeta) UnsetReadyAt()`

UnsetReadyAt ensures that no value is present for ReadyAt, not even an explicit nil
### GetDescription

`func (o *DeploymentVersionMeta) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *DeploymentVersionMeta) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *DeploymentVersionMeta) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *DeploymentVersionMeta) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *DeploymentVersionMeta) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *DeploymentVersionMeta) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetBuildAt

`func (o *DeploymentVersionMeta) GetBuildAt() time.Time`

GetBuildAt returns the BuildAt field if non-nil, zero value otherwise.

### GetBuildAtOk

`func (o *DeploymentVersionMeta) GetBuildAtOk() (*time.Time, bool)`

GetBuildAtOk returns a tuple with the BuildAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildAt

`func (o *DeploymentVersionMeta) SetBuildAt(v time.Time)`

SetBuildAt sets BuildAt field to given value.

### HasBuildAt

`func (o *DeploymentVersionMeta) HasBuildAt() bool`

HasBuildAt returns a boolean if a field has been set.

### SetBuildAtNil

`func (o *DeploymentVersionMeta) SetBuildAtNil(b bool)`

 SetBuildAtNil sets the value for BuildAt to be an explicit nil

### UnsetBuildAt
`func (o *DeploymentVersionMeta) UnsetBuildAt()`

UnsetBuildAt ensures that no value is present for BuildAt, not even an explicit nil
### GetBuildComment

`func (o *DeploymentVersionMeta) GetBuildComment() string`

GetBuildComment returns the BuildComment field if non-nil, zero value otherwise.

### GetBuildCommentOk

`func (o *DeploymentVersionMeta) GetBuildCommentOk() (*string, bool)`

GetBuildCommentOk returns a tuple with the BuildComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildComment

`func (o *DeploymentVersionMeta) SetBuildComment(v string)`

SetBuildComment sets BuildComment field to given value.

### HasBuildComment

`func (o *DeploymentVersionMeta) HasBuildComment() bool`

HasBuildComment returns a boolean if a field has been set.

### SetBuildCommentNil

`func (o *DeploymentVersionMeta) SetBuildCommentNil(b bool)`

 SetBuildCommentNil sets the value for BuildComment to be an explicit nil

### UnsetBuildComment
`func (o *DeploymentVersionMeta) UnsetBuildComment()`

UnsetBuildComment ensures that no value is present for BuildComment, not even an explicit nil
### GetCancelAt

`func (o *DeploymentVersionMeta) GetCancelAt() time.Time`

GetCancelAt returns the CancelAt field if non-nil, zero value otherwise.

### GetCancelAtOk

`func (o *DeploymentVersionMeta) GetCancelAtOk() (*time.Time, bool)`

GetCancelAtOk returns a tuple with the CancelAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelAt

`func (o *DeploymentVersionMeta) SetCancelAt(v time.Time)`

SetCancelAt sets CancelAt field to given value.

### HasCancelAt

`func (o *DeploymentVersionMeta) HasCancelAt() bool`

HasCancelAt returns a boolean if a field has been set.

### SetCancelAtNil

`func (o *DeploymentVersionMeta) SetCancelAtNil(b bool)`

 SetCancelAtNil sets the value for CancelAt to be an explicit nil

### UnsetCancelAt
`func (o *DeploymentVersionMeta) UnsetCancelAt()`

UnsetCancelAt ensures that no value is present for CancelAt, not even an explicit nil
### GetCancelComment

`func (o *DeploymentVersionMeta) GetCancelComment() string`

GetCancelComment returns the CancelComment field if non-nil, zero value otherwise.

### GetCancelCommentOk

`func (o *DeploymentVersionMeta) GetCancelCommentOk() (*string, bool)`

GetCancelCommentOk returns a tuple with the CancelComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelComment

`func (o *DeploymentVersionMeta) SetCancelComment(v string)`

SetCancelComment sets CancelComment field to given value.

### HasCancelComment

`func (o *DeploymentVersionMeta) HasCancelComment() bool`

HasCancelComment returns a boolean if a field has been set.

### SetCancelCommentNil

`func (o *DeploymentVersionMeta) SetCancelCommentNil(b bool)`

 SetCancelCommentNil sets the value for CancelComment to be an explicit nil

### UnsetCancelComment
`func (o *DeploymentVersionMeta) UnsetCancelComment()`

UnsetCancelComment ensures that no value is present for CancelComment, not even an explicit nil
### GetArchivedAt

`func (o *DeploymentVersionMeta) GetArchivedAt() time.Time`

GetArchivedAt returns the ArchivedAt field if non-nil, zero value otherwise.

### GetArchivedAtOk

`func (o *DeploymentVersionMeta) GetArchivedAtOk() (*time.Time, bool)`

GetArchivedAtOk returns a tuple with the ArchivedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchivedAt

`func (o *DeploymentVersionMeta) SetArchivedAt(v time.Time)`

SetArchivedAt sets ArchivedAt field to given value.

### HasArchivedAt

`func (o *DeploymentVersionMeta) HasArchivedAt() bool`

HasArchivedAt returns a boolean if a field has been set.

### SetArchivedAtNil

`func (o *DeploymentVersionMeta) SetArchivedAtNil(b bool)`

 SetArchivedAtNil sets the value for ArchivedAt to be an explicit nil

### UnsetArchivedAt
`func (o *DeploymentVersionMeta) UnsetArchivedAt()`

UnsetArchivedAt ensures that no value is present for ArchivedAt, not even an explicit nil
### GetArchiveComment

`func (o *DeploymentVersionMeta) GetArchiveComment() string`

GetArchiveComment returns the ArchiveComment field if non-nil, zero value otherwise.

### GetArchiveCommentOk

`func (o *DeploymentVersionMeta) GetArchiveCommentOk() (*string, bool)`

GetArchiveCommentOk returns a tuple with the ArchiveComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchiveComment

`func (o *DeploymentVersionMeta) SetArchiveComment(v string)`

SetArchiveComment sets ArchiveComment field to given value.

### HasArchiveComment

`func (o *DeploymentVersionMeta) HasArchiveComment() bool`

HasArchiveComment returns a boolean if a field has been set.

### SetArchiveCommentNil

`func (o *DeploymentVersionMeta) SetArchiveCommentNil(b bool)`

 SetArchiveCommentNil sets the value for ArchiveComment to be an explicit nil

### UnsetArchiveComment
`func (o *DeploymentVersionMeta) UnsetArchiveComment()`

UnsetArchiveComment ensures that no value is present for ArchiveComment, not even an explicit nil
### GetLastError

`func (o *DeploymentVersionMeta) GetLastError() map[string]interface{}`

GetLastError returns the LastError field if non-nil, zero value otherwise.

### GetLastErrorOk

`func (o *DeploymentVersionMeta) GetLastErrorOk() (*map[string]interface{}, bool)`

GetLastErrorOk returns a tuple with the LastError field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastError

`func (o *DeploymentVersionMeta) SetLastError(v map[string]interface{})`

SetLastError sets LastError field to given value.

### HasLastError

`func (o *DeploymentVersionMeta) HasLastError() bool`

HasLastError returns a boolean if a field has been set.

### SetLastErrorNil

`func (o *DeploymentVersionMeta) SetLastErrorNil(b bool)`

 SetLastErrorNil sets the value for LastError to be an explicit nil

### UnsetLastError
`func (o *DeploymentVersionMeta) UnsetLastError()`

UnsetLastError ensures that no value is present for LastError, not even an explicit nil
### GetTraceId

`func (o *DeploymentVersionMeta) GetTraceId() string`

GetTraceId returns the TraceId field if non-nil, zero value otherwise.

### GetTraceIdOk

`func (o *DeploymentVersionMeta) GetTraceIdOk() (*string, bool)`

GetTraceIdOk returns a tuple with the TraceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraceId

`func (o *DeploymentVersionMeta) SetTraceId(v string)`

SetTraceId sets TraceId field to given value.

### HasTraceId

`func (o *DeploymentVersionMeta) HasTraceId() bool`

HasTraceId returns a boolean if a field has been set.

### SetTraceIdNil

`func (o *DeploymentVersionMeta) SetTraceIdNil(b bool)`

 SetTraceIdNil sets the value for TraceId to be an explicit nil

### UnsetTraceId
`func (o *DeploymentVersionMeta) UnsetTraceId()`

UnsetTraceId ensures that no value is present for TraceId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


