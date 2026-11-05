# ConnectorStorageVersion

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** |  | 
**Name** | Pointer to **string** |  | [optional] 
**LastEditor** | Pointer to **string** |  | [optional] 
**LastModified** | Pointer to **time.Time** |  | [optional] 
**Attributes** | Pointer to [**ConnectorStorageAttributes**](ConnectorStorageAttributes.md) |  | [optional] 
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
**Dependencies** | Pointer to [**[]map[string][]ApplicationVersionDependenciesInnerValueInner**](map[string][]ApplicationVersionDependenciesInnerValueInner.md) | Resources this version references, grouped by resource type. Present only when the request sets dependencies&#x3D;true. | [optional] 

## Methods

### NewConnectorStorageVersion

`func NewConnectorStorageVersion(type_ string, ) *ConnectorStorageVersion`

NewConnectorStorageVersion instantiates a new ConnectorStorageVersion object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConnectorStorageVersionWithDefaults

`func NewConnectorStorageVersionWithDefaults() *ConnectorStorageVersion`

NewConnectorStorageVersionWithDefaults instantiates a new ConnectorStorageVersion object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *ConnectorStorageVersion) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ConnectorStorageVersion) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ConnectorStorageVersion) SetType(v string)`

SetType sets Type field to given value.


### GetName

`func (o *ConnectorStorageVersion) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ConnectorStorageVersion) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ConnectorStorageVersion) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ConnectorStorageVersion) HasName() bool`

HasName returns a boolean if a field has been set.

### GetLastEditor

`func (o *ConnectorStorageVersion) GetLastEditor() string`

GetLastEditor returns the LastEditor field if non-nil, zero value otherwise.

### GetLastEditorOk

`func (o *ConnectorStorageVersion) GetLastEditorOk() (*string, bool)`

GetLastEditorOk returns a tuple with the LastEditor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEditor

`func (o *ConnectorStorageVersion) SetLastEditor(v string)`

SetLastEditor sets LastEditor field to given value.

### HasLastEditor

`func (o *ConnectorStorageVersion) HasLastEditor() bool`

HasLastEditor returns a boolean if a field has been set.

### GetLastModified

`func (o *ConnectorStorageVersion) GetLastModified() time.Time`

GetLastModified returns the LastModified field if non-nil, zero value otherwise.

### GetLastModifiedOk

`func (o *ConnectorStorageVersion) GetLastModifiedOk() (*time.Time, bool)`

GetLastModifiedOk returns a tuple with the LastModified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastModified

`func (o *ConnectorStorageVersion) SetLastModified(v time.Time)`

SetLastModified sets LastModified field to given value.

### HasLastModified

`func (o *ConnectorStorageVersion) HasLastModified() bool`

HasLastModified returns a boolean if a field has been set.

### GetAttributes

`func (o *ConnectorStorageVersion) GetAttributes() ConnectorStorageAttributes`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *ConnectorStorageVersion) GetAttributesOk() (*ConnectorStorageAttributes, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *ConnectorStorageVersion) SetAttributes(v ConnectorStorageAttributes)`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *ConnectorStorageVersion) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.

### GetVersionId

`func (o *ConnectorStorageVersion) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *ConnectorStorageVersion) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *ConnectorStorageVersion) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *ConnectorStorageVersion) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### GetVersionState

`func (o *ConnectorStorageVersion) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *ConnectorStorageVersion) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *ConnectorStorageVersion) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *ConnectorStorageVersion) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetProductVersion

`func (o *ConnectorStorageVersion) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *ConnectorStorageVersion) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *ConnectorStorageVersion) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.

### HasProductVersion

`func (o *ConnectorStorageVersion) HasProductVersion() bool`

HasProductVersion returns a boolean if a field has been set.

### GetSourceVersionId

`func (o *ConnectorStorageVersion) GetSourceVersionId() string`

GetSourceVersionId returns the SourceVersionId field if non-nil, zero value otherwise.

### GetSourceVersionIdOk

`func (o *ConnectorStorageVersion) GetSourceVersionIdOk() (*string, bool)`

GetSourceVersionIdOk returns a tuple with the SourceVersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceVersionId

`func (o *ConnectorStorageVersion) SetSourceVersionId(v string)`

SetSourceVersionId sets SourceVersionId field to given value.

### HasSourceVersionId

`func (o *ConnectorStorageVersion) HasSourceVersionId() bool`

HasSourceVersionId returns a boolean if a field has been set.

### SetSourceVersionIdNil

`func (o *ConnectorStorageVersion) SetSourceVersionIdNil(b bool)`

 SetSourceVersionIdNil sets the value for SourceVersionId to be an explicit nil

### UnsetSourceVersionId
`func (o *ConnectorStorageVersion) UnsetSourceVersionId()`

UnsetSourceVersionId ensures that no value is present for SourceVersionId, not even an explicit nil
### GetSnapshot

`func (o *ConnectorStorageVersion) GetSnapshot() map[string]interface{}`

GetSnapshot returns the Snapshot field if non-nil, zero value otherwise.

### GetSnapshotOk

`func (o *ConnectorStorageVersion) GetSnapshotOk() (*map[string]interface{}, bool)`

GetSnapshotOk returns a tuple with the Snapshot field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnapshot

`func (o *ConnectorStorageVersion) SetSnapshot(v map[string]interface{})`

SetSnapshot sets Snapshot field to given value.

### HasSnapshot

`func (o *ConnectorStorageVersion) HasSnapshot() bool`

HasSnapshot returns a boolean if a field has been set.

### SetSnapshotNil

`func (o *ConnectorStorageVersion) SetSnapshotNil(b bool)`

 SetSnapshotNil sets the value for Snapshot to be an explicit nil

### UnsetSnapshot
`func (o *ConnectorStorageVersion) UnsetSnapshot()`

UnsetSnapshot ensures that no value is present for Snapshot, not even an explicit nil
### GetCreatedAt

`func (o *ConnectorStorageVersion) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *ConnectorStorageVersion) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *ConnectorStorageVersion) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *ConnectorStorageVersion) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetReadyAt

`func (o *ConnectorStorageVersion) GetReadyAt() time.Time`

GetReadyAt returns the ReadyAt field if non-nil, zero value otherwise.

### GetReadyAtOk

`func (o *ConnectorStorageVersion) GetReadyAtOk() (*time.Time, bool)`

GetReadyAtOk returns a tuple with the ReadyAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadyAt

`func (o *ConnectorStorageVersion) SetReadyAt(v time.Time)`

SetReadyAt sets ReadyAt field to given value.

### HasReadyAt

`func (o *ConnectorStorageVersion) HasReadyAt() bool`

HasReadyAt returns a boolean if a field has been set.

### SetReadyAtNil

`func (o *ConnectorStorageVersion) SetReadyAtNil(b bool)`

 SetReadyAtNil sets the value for ReadyAt to be an explicit nil

### UnsetReadyAt
`func (o *ConnectorStorageVersion) UnsetReadyAt()`

UnsetReadyAt ensures that no value is present for ReadyAt, not even an explicit nil
### GetDescription

`func (o *ConnectorStorageVersion) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ConnectorStorageVersion) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ConnectorStorageVersion) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ConnectorStorageVersion) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetBuildAt

`func (o *ConnectorStorageVersion) GetBuildAt() time.Time`

GetBuildAt returns the BuildAt field if non-nil, zero value otherwise.

### GetBuildAtOk

`func (o *ConnectorStorageVersion) GetBuildAtOk() (*time.Time, bool)`

GetBuildAtOk returns a tuple with the BuildAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildAt

`func (o *ConnectorStorageVersion) SetBuildAt(v time.Time)`

SetBuildAt sets BuildAt field to given value.

### HasBuildAt

`func (o *ConnectorStorageVersion) HasBuildAt() bool`

HasBuildAt returns a boolean if a field has been set.

### SetBuildAtNil

`func (o *ConnectorStorageVersion) SetBuildAtNil(b bool)`

 SetBuildAtNil sets the value for BuildAt to be an explicit nil

### UnsetBuildAt
`func (o *ConnectorStorageVersion) UnsetBuildAt()`

UnsetBuildAt ensures that no value is present for BuildAt, not even an explicit nil
### GetBuildComment

`func (o *ConnectorStorageVersion) GetBuildComment() string`

GetBuildComment returns the BuildComment field if non-nil, zero value otherwise.

### GetBuildCommentOk

`func (o *ConnectorStorageVersion) GetBuildCommentOk() (*string, bool)`

GetBuildCommentOk returns a tuple with the BuildComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildComment

`func (o *ConnectorStorageVersion) SetBuildComment(v string)`

SetBuildComment sets BuildComment field to given value.

### HasBuildComment

`func (o *ConnectorStorageVersion) HasBuildComment() bool`

HasBuildComment returns a boolean if a field has been set.

### GetCancelAt

`func (o *ConnectorStorageVersion) GetCancelAt() time.Time`

GetCancelAt returns the CancelAt field if non-nil, zero value otherwise.

### GetCancelAtOk

`func (o *ConnectorStorageVersion) GetCancelAtOk() (*time.Time, bool)`

GetCancelAtOk returns a tuple with the CancelAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelAt

`func (o *ConnectorStorageVersion) SetCancelAt(v time.Time)`

SetCancelAt sets CancelAt field to given value.

### HasCancelAt

`func (o *ConnectorStorageVersion) HasCancelAt() bool`

HasCancelAt returns a boolean if a field has been set.

### SetCancelAtNil

`func (o *ConnectorStorageVersion) SetCancelAtNil(b bool)`

 SetCancelAtNil sets the value for CancelAt to be an explicit nil

### UnsetCancelAt
`func (o *ConnectorStorageVersion) UnsetCancelAt()`

UnsetCancelAt ensures that no value is present for CancelAt, not even an explicit nil
### GetCancelComment

`func (o *ConnectorStorageVersion) GetCancelComment() string`

GetCancelComment returns the CancelComment field if non-nil, zero value otherwise.

### GetCancelCommentOk

`func (o *ConnectorStorageVersion) GetCancelCommentOk() (*string, bool)`

GetCancelCommentOk returns a tuple with the CancelComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelComment

`func (o *ConnectorStorageVersion) SetCancelComment(v string)`

SetCancelComment sets CancelComment field to given value.

### HasCancelComment

`func (o *ConnectorStorageVersion) HasCancelComment() bool`

HasCancelComment returns a boolean if a field has been set.

### GetArchivedAt

`func (o *ConnectorStorageVersion) GetArchivedAt() time.Time`

GetArchivedAt returns the ArchivedAt field if non-nil, zero value otherwise.

### GetArchivedAtOk

`func (o *ConnectorStorageVersion) GetArchivedAtOk() (*time.Time, bool)`

GetArchivedAtOk returns a tuple with the ArchivedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchivedAt

`func (o *ConnectorStorageVersion) SetArchivedAt(v time.Time)`

SetArchivedAt sets ArchivedAt field to given value.

### HasArchivedAt

`func (o *ConnectorStorageVersion) HasArchivedAt() bool`

HasArchivedAt returns a boolean if a field has been set.

### SetArchivedAtNil

`func (o *ConnectorStorageVersion) SetArchivedAtNil(b bool)`

 SetArchivedAtNil sets the value for ArchivedAt to be an explicit nil

### UnsetArchivedAt
`func (o *ConnectorStorageVersion) UnsetArchivedAt()`

UnsetArchivedAt ensures that no value is present for ArchivedAt, not even an explicit nil
### GetArchiveComment

`func (o *ConnectorStorageVersion) GetArchiveComment() string`

GetArchiveComment returns the ArchiveComment field if non-nil, zero value otherwise.

### GetArchiveCommentOk

`func (o *ConnectorStorageVersion) GetArchiveCommentOk() (*string, bool)`

GetArchiveCommentOk returns a tuple with the ArchiveComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchiveComment

`func (o *ConnectorStorageVersion) SetArchiveComment(v string)`

SetArchiveComment sets ArchiveComment field to given value.

### HasArchiveComment

`func (o *ConnectorStorageVersion) HasArchiveComment() bool`

HasArchiveComment returns a boolean if a field has been set.

### GetLastError

`func (o *ConnectorStorageVersion) GetLastError() map[string]interface{}`

GetLastError returns the LastError field if non-nil, zero value otherwise.

### GetLastErrorOk

`func (o *ConnectorStorageVersion) GetLastErrorOk() (*map[string]interface{}, bool)`

GetLastErrorOk returns a tuple with the LastError field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastError

`func (o *ConnectorStorageVersion) SetLastError(v map[string]interface{})`

SetLastError sets LastError field to given value.

### HasLastError

`func (o *ConnectorStorageVersion) HasLastError() bool`

HasLastError returns a boolean if a field has been set.

### SetLastErrorNil

`func (o *ConnectorStorageVersion) SetLastErrorNil(b bool)`

 SetLastErrorNil sets the value for LastError to be an explicit nil

### UnsetLastError
`func (o *ConnectorStorageVersion) UnsetLastError()`

UnsetLastError ensures that no value is present for LastError, not even an explicit nil
### GetTraceId

`func (o *ConnectorStorageVersion) GetTraceId() string`

GetTraceId returns the TraceId field if non-nil, zero value otherwise.

### GetTraceIdOk

`func (o *ConnectorStorageVersion) GetTraceIdOk() (*string, bool)`

GetTraceIdOk returns a tuple with the TraceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraceId

`func (o *ConnectorStorageVersion) SetTraceId(v string)`

SetTraceId sets TraceId field to given value.

### HasTraceId

`func (o *ConnectorStorageVersion) HasTraceId() bool`

HasTraceId returns a boolean if a field has been set.

### GetDependencies

`func (o *ConnectorStorageVersion) GetDependencies() []map[string][]ApplicationVersionDependenciesInnerValueInner`

GetDependencies returns the Dependencies field if non-nil, zero value otherwise.

### GetDependenciesOk

`func (o *ConnectorStorageVersion) GetDependenciesOk() (*[]map[string][]ApplicationVersionDependenciesInnerValueInner, bool)`

GetDependenciesOk returns a tuple with the Dependencies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDependencies

`func (o *ConnectorStorageVersion) SetDependencies(v []map[string][]ApplicationVersionDependenciesInnerValueInner)`

SetDependencies sets Dependencies field to given value.

### HasDependencies

`func (o *ConnectorStorageVersion) HasDependencies() bool`

HasDependencies returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


