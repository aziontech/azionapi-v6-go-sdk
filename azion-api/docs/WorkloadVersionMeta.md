# WorkloadVersionMeta

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**VersionId** | Pointer to **string** | ID of the version metadata | [optional] 
**VersionState** | Pointer to **string** | Current lifecycle state of the version. | [optional] 
**ProductVersion** | Pointer to **string** | Product version string | [optional] 
**SourceVersionId** | Pointer to **NullableString** | ID of the source version if cloned | [optional] 
**Snapshot** | Pointer to **map[string]interface{}** | JSON snapshot of the version data | [optional] 
**CreatedAt** | Pointer to **time.Time** | When this version was created | [optional] 
**ReadyAt** | Pointer to **NullableTime** | When this version became ready | [optional] 
**Description** | Pointer to **string** | Version description | [optional] 
**BuildAt** | Pointer to **NullableTime** | When a build was triggered | [optional] 
**BuildComment** | Pointer to **string** | Comment provided when triggering the build | [optional] 
**CancelAt** | Pointer to **NullableTime** | When a cancel was triggered | [optional] 
**CancelComment** | Pointer to **string** | Comment provided when cancelling the build | [optional] 
**ArchivedAt** | Pointer to **NullableTime** | When this version was archived | [optional] 
**ArchiveComment** | Pointer to **string** | Comment provided when archiving | [optional] 
**LastError** | Pointer to **map[string]interface{}** | Last build error details | [optional] 
**TraceId** | Pointer to **string** | Trace ID of the last build, for observability. Omitted when unset. | [optional] 

## Methods

### NewWorkloadVersionMeta

`func NewWorkloadVersionMeta() *WorkloadVersionMeta`

NewWorkloadVersionMeta instantiates a new WorkloadVersionMeta object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWorkloadVersionMetaWithDefaults

`func NewWorkloadVersionMetaWithDefaults() *WorkloadVersionMeta`

NewWorkloadVersionMetaWithDefaults instantiates a new WorkloadVersionMeta object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersionId

`func (o *WorkloadVersionMeta) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *WorkloadVersionMeta) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *WorkloadVersionMeta) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *WorkloadVersionMeta) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### GetVersionState

`func (o *WorkloadVersionMeta) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *WorkloadVersionMeta) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *WorkloadVersionMeta) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *WorkloadVersionMeta) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetProductVersion

`func (o *WorkloadVersionMeta) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *WorkloadVersionMeta) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *WorkloadVersionMeta) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.

### HasProductVersion

`func (o *WorkloadVersionMeta) HasProductVersion() bool`

HasProductVersion returns a boolean if a field has been set.

### GetSourceVersionId

`func (o *WorkloadVersionMeta) GetSourceVersionId() string`

GetSourceVersionId returns the SourceVersionId field if non-nil, zero value otherwise.

### GetSourceVersionIdOk

`func (o *WorkloadVersionMeta) GetSourceVersionIdOk() (*string, bool)`

GetSourceVersionIdOk returns a tuple with the SourceVersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceVersionId

`func (o *WorkloadVersionMeta) SetSourceVersionId(v string)`

SetSourceVersionId sets SourceVersionId field to given value.

### HasSourceVersionId

`func (o *WorkloadVersionMeta) HasSourceVersionId() bool`

HasSourceVersionId returns a boolean if a field has been set.

### SetSourceVersionIdNil

`func (o *WorkloadVersionMeta) SetSourceVersionIdNil(b bool)`

 SetSourceVersionIdNil sets the value for SourceVersionId to be an explicit nil

### UnsetSourceVersionId
`func (o *WorkloadVersionMeta) UnsetSourceVersionId()`

UnsetSourceVersionId ensures that no value is present for SourceVersionId, not even an explicit nil
### GetSnapshot

`func (o *WorkloadVersionMeta) GetSnapshot() map[string]interface{}`

GetSnapshot returns the Snapshot field if non-nil, zero value otherwise.

### GetSnapshotOk

`func (o *WorkloadVersionMeta) GetSnapshotOk() (*map[string]interface{}, bool)`

GetSnapshotOk returns a tuple with the Snapshot field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnapshot

`func (o *WorkloadVersionMeta) SetSnapshot(v map[string]interface{})`

SetSnapshot sets Snapshot field to given value.

### HasSnapshot

`func (o *WorkloadVersionMeta) HasSnapshot() bool`

HasSnapshot returns a boolean if a field has been set.

### SetSnapshotNil

`func (o *WorkloadVersionMeta) SetSnapshotNil(b bool)`

 SetSnapshotNil sets the value for Snapshot to be an explicit nil

### UnsetSnapshot
`func (o *WorkloadVersionMeta) UnsetSnapshot()`

UnsetSnapshot ensures that no value is present for Snapshot, not even an explicit nil
### GetCreatedAt

`func (o *WorkloadVersionMeta) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *WorkloadVersionMeta) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *WorkloadVersionMeta) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *WorkloadVersionMeta) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetReadyAt

`func (o *WorkloadVersionMeta) GetReadyAt() time.Time`

GetReadyAt returns the ReadyAt field if non-nil, zero value otherwise.

### GetReadyAtOk

`func (o *WorkloadVersionMeta) GetReadyAtOk() (*time.Time, bool)`

GetReadyAtOk returns a tuple with the ReadyAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadyAt

`func (o *WorkloadVersionMeta) SetReadyAt(v time.Time)`

SetReadyAt sets ReadyAt field to given value.

### HasReadyAt

`func (o *WorkloadVersionMeta) HasReadyAt() bool`

HasReadyAt returns a boolean if a field has been set.

### SetReadyAtNil

`func (o *WorkloadVersionMeta) SetReadyAtNil(b bool)`

 SetReadyAtNil sets the value for ReadyAt to be an explicit nil

### UnsetReadyAt
`func (o *WorkloadVersionMeta) UnsetReadyAt()`

UnsetReadyAt ensures that no value is present for ReadyAt, not even an explicit nil
### GetDescription

`func (o *WorkloadVersionMeta) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *WorkloadVersionMeta) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *WorkloadVersionMeta) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *WorkloadVersionMeta) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetBuildAt

`func (o *WorkloadVersionMeta) GetBuildAt() time.Time`

GetBuildAt returns the BuildAt field if non-nil, zero value otherwise.

### GetBuildAtOk

`func (o *WorkloadVersionMeta) GetBuildAtOk() (*time.Time, bool)`

GetBuildAtOk returns a tuple with the BuildAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildAt

`func (o *WorkloadVersionMeta) SetBuildAt(v time.Time)`

SetBuildAt sets BuildAt field to given value.

### HasBuildAt

`func (o *WorkloadVersionMeta) HasBuildAt() bool`

HasBuildAt returns a boolean if a field has been set.

### SetBuildAtNil

`func (o *WorkloadVersionMeta) SetBuildAtNil(b bool)`

 SetBuildAtNil sets the value for BuildAt to be an explicit nil

### UnsetBuildAt
`func (o *WorkloadVersionMeta) UnsetBuildAt()`

UnsetBuildAt ensures that no value is present for BuildAt, not even an explicit nil
### GetBuildComment

`func (o *WorkloadVersionMeta) GetBuildComment() string`

GetBuildComment returns the BuildComment field if non-nil, zero value otherwise.

### GetBuildCommentOk

`func (o *WorkloadVersionMeta) GetBuildCommentOk() (*string, bool)`

GetBuildCommentOk returns a tuple with the BuildComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildComment

`func (o *WorkloadVersionMeta) SetBuildComment(v string)`

SetBuildComment sets BuildComment field to given value.

### HasBuildComment

`func (o *WorkloadVersionMeta) HasBuildComment() bool`

HasBuildComment returns a boolean if a field has been set.

### GetCancelAt

`func (o *WorkloadVersionMeta) GetCancelAt() time.Time`

GetCancelAt returns the CancelAt field if non-nil, zero value otherwise.

### GetCancelAtOk

`func (o *WorkloadVersionMeta) GetCancelAtOk() (*time.Time, bool)`

GetCancelAtOk returns a tuple with the CancelAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelAt

`func (o *WorkloadVersionMeta) SetCancelAt(v time.Time)`

SetCancelAt sets CancelAt field to given value.

### HasCancelAt

`func (o *WorkloadVersionMeta) HasCancelAt() bool`

HasCancelAt returns a boolean if a field has been set.

### SetCancelAtNil

`func (o *WorkloadVersionMeta) SetCancelAtNil(b bool)`

 SetCancelAtNil sets the value for CancelAt to be an explicit nil

### UnsetCancelAt
`func (o *WorkloadVersionMeta) UnsetCancelAt()`

UnsetCancelAt ensures that no value is present for CancelAt, not even an explicit nil
### GetCancelComment

`func (o *WorkloadVersionMeta) GetCancelComment() string`

GetCancelComment returns the CancelComment field if non-nil, zero value otherwise.

### GetCancelCommentOk

`func (o *WorkloadVersionMeta) GetCancelCommentOk() (*string, bool)`

GetCancelCommentOk returns a tuple with the CancelComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelComment

`func (o *WorkloadVersionMeta) SetCancelComment(v string)`

SetCancelComment sets CancelComment field to given value.

### HasCancelComment

`func (o *WorkloadVersionMeta) HasCancelComment() bool`

HasCancelComment returns a boolean if a field has been set.

### GetArchivedAt

`func (o *WorkloadVersionMeta) GetArchivedAt() time.Time`

GetArchivedAt returns the ArchivedAt field if non-nil, zero value otherwise.

### GetArchivedAtOk

`func (o *WorkloadVersionMeta) GetArchivedAtOk() (*time.Time, bool)`

GetArchivedAtOk returns a tuple with the ArchivedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchivedAt

`func (o *WorkloadVersionMeta) SetArchivedAt(v time.Time)`

SetArchivedAt sets ArchivedAt field to given value.

### HasArchivedAt

`func (o *WorkloadVersionMeta) HasArchivedAt() bool`

HasArchivedAt returns a boolean if a field has been set.

### SetArchivedAtNil

`func (o *WorkloadVersionMeta) SetArchivedAtNil(b bool)`

 SetArchivedAtNil sets the value for ArchivedAt to be an explicit nil

### UnsetArchivedAt
`func (o *WorkloadVersionMeta) UnsetArchivedAt()`

UnsetArchivedAt ensures that no value is present for ArchivedAt, not even an explicit nil
### GetArchiveComment

`func (o *WorkloadVersionMeta) GetArchiveComment() string`

GetArchiveComment returns the ArchiveComment field if non-nil, zero value otherwise.

### GetArchiveCommentOk

`func (o *WorkloadVersionMeta) GetArchiveCommentOk() (*string, bool)`

GetArchiveCommentOk returns a tuple with the ArchiveComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchiveComment

`func (o *WorkloadVersionMeta) SetArchiveComment(v string)`

SetArchiveComment sets ArchiveComment field to given value.

### HasArchiveComment

`func (o *WorkloadVersionMeta) HasArchiveComment() bool`

HasArchiveComment returns a boolean if a field has been set.

### GetLastError

`func (o *WorkloadVersionMeta) GetLastError() map[string]interface{}`

GetLastError returns the LastError field if non-nil, zero value otherwise.

### GetLastErrorOk

`func (o *WorkloadVersionMeta) GetLastErrorOk() (*map[string]interface{}, bool)`

GetLastErrorOk returns a tuple with the LastError field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastError

`func (o *WorkloadVersionMeta) SetLastError(v map[string]interface{})`

SetLastError sets LastError field to given value.

### HasLastError

`func (o *WorkloadVersionMeta) HasLastError() bool`

HasLastError returns a boolean if a field has been set.

### SetLastErrorNil

`func (o *WorkloadVersionMeta) SetLastErrorNil(b bool)`

 SetLastErrorNil sets the value for LastError to be an explicit nil

### UnsetLastError
`func (o *WorkloadVersionMeta) UnsetLastError()`

UnsetLastError ensures that no value is present for LastError, not even an explicit nil
### GetTraceId

`func (o *WorkloadVersionMeta) GetTraceId() string`

GetTraceId returns the TraceId field if non-nil, zero value otherwise.

### GetTraceIdOk

`func (o *WorkloadVersionMeta) GetTraceIdOk() (*string, bool)`

GetTraceIdOk returns a tuple with the TraceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraceId

`func (o *WorkloadVersionMeta) SetTraceId(v string)`

SetTraceId sets TraceId field to given value.

### HasTraceId

`func (o *WorkloadVersionMeta) HasTraceId() bool`

HasTraceId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


