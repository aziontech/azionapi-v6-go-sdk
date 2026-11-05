# FunctionVersionMeta

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

### NewFunctionVersionMeta

`func NewFunctionVersionMeta() *FunctionVersionMeta`

NewFunctionVersionMeta instantiates a new FunctionVersionMeta object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFunctionVersionMetaWithDefaults

`func NewFunctionVersionMetaWithDefaults() *FunctionVersionMeta`

NewFunctionVersionMetaWithDefaults instantiates a new FunctionVersionMeta object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersionId

`func (o *FunctionVersionMeta) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *FunctionVersionMeta) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *FunctionVersionMeta) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *FunctionVersionMeta) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### GetVersionState

`func (o *FunctionVersionMeta) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *FunctionVersionMeta) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *FunctionVersionMeta) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *FunctionVersionMeta) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetProductVersion

`func (o *FunctionVersionMeta) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *FunctionVersionMeta) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *FunctionVersionMeta) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.

### HasProductVersion

`func (o *FunctionVersionMeta) HasProductVersion() bool`

HasProductVersion returns a boolean if a field has been set.

### GetSourceVersionId

`func (o *FunctionVersionMeta) GetSourceVersionId() string`

GetSourceVersionId returns the SourceVersionId field if non-nil, zero value otherwise.

### GetSourceVersionIdOk

`func (o *FunctionVersionMeta) GetSourceVersionIdOk() (*string, bool)`

GetSourceVersionIdOk returns a tuple with the SourceVersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceVersionId

`func (o *FunctionVersionMeta) SetSourceVersionId(v string)`

SetSourceVersionId sets SourceVersionId field to given value.

### HasSourceVersionId

`func (o *FunctionVersionMeta) HasSourceVersionId() bool`

HasSourceVersionId returns a boolean if a field has been set.

### SetSourceVersionIdNil

`func (o *FunctionVersionMeta) SetSourceVersionIdNil(b bool)`

 SetSourceVersionIdNil sets the value for SourceVersionId to be an explicit nil

### UnsetSourceVersionId
`func (o *FunctionVersionMeta) UnsetSourceVersionId()`

UnsetSourceVersionId ensures that no value is present for SourceVersionId, not even an explicit nil
### GetSnapshot

`func (o *FunctionVersionMeta) GetSnapshot() map[string]interface{}`

GetSnapshot returns the Snapshot field if non-nil, zero value otherwise.

### GetSnapshotOk

`func (o *FunctionVersionMeta) GetSnapshotOk() (*map[string]interface{}, bool)`

GetSnapshotOk returns a tuple with the Snapshot field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnapshot

`func (o *FunctionVersionMeta) SetSnapshot(v map[string]interface{})`

SetSnapshot sets Snapshot field to given value.

### HasSnapshot

`func (o *FunctionVersionMeta) HasSnapshot() bool`

HasSnapshot returns a boolean if a field has been set.

### SetSnapshotNil

`func (o *FunctionVersionMeta) SetSnapshotNil(b bool)`

 SetSnapshotNil sets the value for Snapshot to be an explicit nil

### UnsetSnapshot
`func (o *FunctionVersionMeta) UnsetSnapshot()`

UnsetSnapshot ensures that no value is present for Snapshot, not even an explicit nil
### GetCreatedAt

`func (o *FunctionVersionMeta) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *FunctionVersionMeta) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *FunctionVersionMeta) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *FunctionVersionMeta) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetReadyAt

`func (o *FunctionVersionMeta) GetReadyAt() time.Time`

GetReadyAt returns the ReadyAt field if non-nil, zero value otherwise.

### GetReadyAtOk

`func (o *FunctionVersionMeta) GetReadyAtOk() (*time.Time, bool)`

GetReadyAtOk returns a tuple with the ReadyAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadyAt

`func (o *FunctionVersionMeta) SetReadyAt(v time.Time)`

SetReadyAt sets ReadyAt field to given value.

### HasReadyAt

`func (o *FunctionVersionMeta) HasReadyAt() bool`

HasReadyAt returns a boolean if a field has been set.

### SetReadyAtNil

`func (o *FunctionVersionMeta) SetReadyAtNil(b bool)`

 SetReadyAtNil sets the value for ReadyAt to be an explicit nil

### UnsetReadyAt
`func (o *FunctionVersionMeta) UnsetReadyAt()`

UnsetReadyAt ensures that no value is present for ReadyAt, not even an explicit nil
### GetDescription

`func (o *FunctionVersionMeta) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *FunctionVersionMeta) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *FunctionVersionMeta) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *FunctionVersionMeta) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetBuildAt

`func (o *FunctionVersionMeta) GetBuildAt() time.Time`

GetBuildAt returns the BuildAt field if non-nil, zero value otherwise.

### GetBuildAtOk

`func (o *FunctionVersionMeta) GetBuildAtOk() (*time.Time, bool)`

GetBuildAtOk returns a tuple with the BuildAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildAt

`func (o *FunctionVersionMeta) SetBuildAt(v time.Time)`

SetBuildAt sets BuildAt field to given value.

### HasBuildAt

`func (o *FunctionVersionMeta) HasBuildAt() bool`

HasBuildAt returns a boolean if a field has been set.

### SetBuildAtNil

`func (o *FunctionVersionMeta) SetBuildAtNil(b bool)`

 SetBuildAtNil sets the value for BuildAt to be an explicit nil

### UnsetBuildAt
`func (o *FunctionVersionMeta) UnsetBuildAt()`

UnsetBuildAt ensures that no value is present for BuildAt, not even an explicit nil
### GetBuildComment

`func (o *FunctionVersionMeta) GetBuildComment() string`

GetBuildComment returns the BuildComment field if non-nil, zero value otherwise.

### GetBuildCommentOk

`func (o *FunctionVersionMeta) GetBuildCommentOk() (*string, bool)`

GetBuildCommentOk returns a tuple with the BuildComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildComment

`func (o *FunctionVersionMeta) SetBuildComment(v string)`

SetBuildComment sets BuildComment field to given value.

### HasBuildComment

`func (o *FunctionVersionMeta) HasBuildComment() bool`

HasBuildComment returns a boolean if a field has been set.

### GetCancelAt

`func (o *FunctionVersionMeta) GetCancelAt() time.Time`

GetCancelAt returns the CancelAt field if non-nil, zero value otherwise.

### GetCancelAtOk

`func (o *FunctionVersionMeta) GetCancelAtOk() (*time.Time, bool)`

GetCancelAtOk returns a tuple with the CancelAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelAt

`func (o *FunctionVersionMeta) SetCancelAt(v time.Time)`

SetCancelAt sets CancelAt field to given value.

### HasCancelAt

`func (o *FunctionVersionMeta) HasCancelAt() bool`

HasCancelAt returns a boolean if a field has been set.

### SetCancelAtNil

`func (o *FunctionVersionMeta) SetCancelAtNil(b bool)`

 SetCancelAtNil sets the value for CancelAt to be an explicit nil

### UnsetCancelAt
`func (o *FunctionVersionMeta) UnsetCancelAt()`

UnsetCancelAt ensures that no value is present for CancelAt, not even an explicit nil
### GetCancelComment

`func (o *FunctionVersionMeta) GetCancelComment() string`

GetCancelComment returns the CancelComment field if non-nil, zero value otherwise.

### GetCancelCommentOk

`func (o *FunctionVersionMeta) GetCancelCommentOk() (*string, bool)`

GetCancelCommentOk returns a tuple with the CancelComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelComment

`func (o *FunctionVersionMeta) SetCancelComment(v string)`

SetCancelComment sets CancelComment field to given value.

### HasCancelComment

`func (o *FunctionVersionMeta) HasCancelComment() bool`

HasCancelComment returns a boolean if a field has been set.

### GetArchivedAt

`func (o *FunctionVersionMeta) GetArchivedAt() time.Time`

GetArchivedAt returns the ArchivedAt field if non-nil, zero value otherwise.

### GetArchivedAtOk

`func (o *FunctionVersionMeta) GetArchivedAtOk() (*time.Time, bool)`

GetArchivedAtOk returns a tuple with the ArchivedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchivedAt

`func (o *FunctionVersionMeta) SetArchivedAt(v time.Time)`

SetArchivedAt sets ArchivedAt field to given value.

### HasArchivedAt

`func (o *FunctionVersionMeta) HasArchivedAt() bool`

HasArchivedAt returns a boolean if a field has been set.

### SetArchivedAtNil

`func (o *FunctionVersionMeta) SetArchivedAtNil(b bool)`

 SetArchivedAtNil sets the value for ArchivedAt to be an explicit nil

### UnsetArchivedAt
`func (o *FunctionVersionMeta) UnsetArchivedAt()`

UnsetArchivedAt ensures that no value is present for ArchivedAt, not even an explicit nil
### GetArchiveComment

`func (o *FunctionVersionMeta) GetArchiveComment() string`

GetArchiveComment returns the ArchiveComment field if non-nil, zero value otherwise.

### GetArchiveCommentOk

`func (o *FunctionVersionMeta) GetArchiveCommentOk() (*string, bool)`

GetArchiveCommentOk returns a tuple with the ArchiveComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchiveComment

`func (o *FunctionVersionMeta) SetArchiveComment(v string)`

SetArchiveComment sets ArchiveComment field to given value.

### HasArchiveComment

`func (o *FunctionVersionMeta) HasArchiveComment() bool`

HasArchiveComment returns a boolean if a field has been set.

### GetLastError

`func (o *FunctionVersionMeta) GetLastError() map[string]interface{}`

GetLastError returns the LastError field if non-nil, zero value otherwise.

### GetLastErrorOk

`func (o *FunctionVersionMeta) GetLastErrorOk() (*map[string]interface{}, bool)`

GetLastErrorOk returns a tuple with the LastError field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastError

`func (o *FunctionVersionMeta) SetLastError(v map[string]interface{})`

SetLastError sets LastError field to given value.

### HasLastError

`func (o *FunctionVersionMeta) HasLastError() bool`

HasLastError returns a boolean if a field has been set.

### SetLastErrorNil

`func (o *FunctionVersionMeta) SetLastErrorNil(b bool)`

 SetLastErrorNil sets the value for LastError to be an explicit nil

### UnsetLastError
`func (o *FunctionVersionMeta) UnsetLastError()`

UnsetLastError ensures that no value is present for LastError, not even an explicit nil
### GetTraceId

`func (o *FunctionVersionMeta) GetTraceId() string`

GetTraceId returns the TraceId field if non-nil, zero value otherwise.

### GetTraceIdOk

`func (o *FunctionVersionMeta) GetTraceIdOk() (*string, bool)`

GetTraceIdOk returns a tuple with the TraceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraceId

`func (o *FunctionVersionMeta) SetTraceId(v string)`

SetTraceId sets TraceId field to given value.

### HasTraceId

`func (o *FunctionVersionMeta) HasTraceId() bool`

HasTraceId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


