# ConnectorHTTPVersion

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** |  | 
**Name** | Pointer to **string** |  | [optional] 
**LastEditor** | Pointer to **string** |  | [optional] 
**LastModified** | Pointer to **time.Time** |  | [optional] 
**Attributes** | Pointer to [**ConnectorHTTPAttributes**](ConnectorHTTPAttributes.md) |  | [optional] 
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

### NewConnectorHTTPVersion

`func NewConnectorHTTPVersion(type_ string, ) *ConnectorHTTPVersion`

NewConnectorHTTPVersion instantiates a new ConnectorHTTPVersion object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConnectorHTTPVersionWithDefaults

`func NewConnectorHTTPVersionWithDefaults() *ConnectorHTTPVersion`

NewConnectorHTTPVersionWithDefaults instantiates a new ConnectorHTTPVersion object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *ConnectorHTTPVersion) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ConnectorHTTPVersion) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ConnectorHTTPVersion) SetType(v string)`

SetType sets Type field to given value.


### GetName

`func (o *ConnectorHTTPVersion) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ConnectorHTTPVersion) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ConnectorHTTPVersion) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ConnectorHTTPVersion) HasName() bool`

HasName returns a boolean if a field has been set.

### GetLastEditor

`func (o *ConnectorHTTPVersion) GetLastEditor() string`

GetLastEditor returns the LastEditor field if non-nil, zero value otherwise.

### GetLastEditorOk

`func (o *ConnectorHTTPVersion) GetLastEditorOk() (*string, bool)`

GetLastEditorOk returns a tuple with the LastEditor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEditor

`func (o *ConnectorHTTPVersion) SetLastEditor(v string)`

SetLastEditor sets LastEditor field to given value.

### HasLastEditor

`func (o *ConnectorHTTPVersion) HasLastEditor() bool`

HasLastEditor returns a boolean if a field has been set.

### GetLastModified

`func (o *ConnectorHTTPVersion) GetLastModified() time.Time`

GetLastModified returns the LastModified field if non-nil, zero value otherwise.

### GetLastModifiedOk

`func (o *ConnectorHTTPVersion) GetLastModifiedOk() (*time.Time, bool)`

GetLastModifiedOk returns a tuple with the LastModified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastModified

`func (o *ConnectorHTTPVersion) SetLastModified(v time.Time)`

SetLastModified sets LastModified field to given value.

### HasLastModified

`func (o *ConnectorHTTPVersion) HasLastModified() bool`

HasLastModified returns a boolean if a field has been set.

### GetAttributes

`func (o *ConnectorHTTPVersion) GetAttributes() ConnectorHTTPAttributes`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *ConnectorHTTPVersion) GetAttributesOk() (*ConnectorHTTPAttributes, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *ConnectorHTTPVersion) SetAttributes(v ConnectorHTTPAttributes)`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *ConnectorHTTPVersion) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.

### GetVersionId

`func (o *ConnectorHTTPVersion) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *ConnectorHTTPVersion) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *ConnectorHTTPVersion) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *ConnectorHTTPVersion) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### GetVersionState

`func (o *ConnectorHTTPVersion) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *ConnectorHTTPVersion) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *ConnectorHTTPVersion) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *ConnectorHTTPVersion) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetProductVersion

`func (o *ConnectorHTTPVersion) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *ConnectorHTTPVersion) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *ConnectorHTTPVersion) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.

### HasProductVersion

`func (o *ConnectorHTTPVersion) HasProductVersion() bool`

HasProductVersion returns a boolean if a field has been set.

### GetSourceVersionId

`func (o *ConnectorHTTPVersion) GetSourceVersionId() string`

GetSourceVersionId returns the SourceVersionId field if non-nil, zero value otherwise.

### GetSourceVersionIdOk

`func (o *ConnectorHTTPVersion) GetSourceVersionIdOk() (*string, bool)`

GetSourceVersionIdOk returns a tuple with the SourceVersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceVersionId

`func (o *ConnectorHTTPVersion) SetSourceVersionId(v string)`

SetSourceVersionId sets SourceVersionId field to given value.

### HasSourceVersionId

`func (o *ConnectorHTTPVersion) HasSourceVersionId() bool`

HasSourceVersionId returns a boolean if a field has been set.

### SetSourceVersionIdNil

`func (o *ConnectorHTTPVersion) SetSourceVersionIdNil(b bool)`

 SetSourceVersionIdNil sets the value for SourceVersionId to be an explicit nil

### UnsetSourceVersionId
`func (o *ConnectorHTTPVersion) UnsetSourceVersionId()`

UnsetSourceVersionId ensures that no value is present for SourceVersionId, not even an explicit nil
### GetSnapshot

`func (o *ConnectorHTTPVersion) GetSnapshot() map[string]interface{}`

GetSnapshot returns the Snapshot field if non-nil, zero value otherwise.

### GetSnapshotOk

`func (o *ConnectorHTTPVersion) GetSnapshotOk() (*map[string]interface{}, bool)`

GetSnapshotOk returns a tuple with the Snapshot field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnapshot

`func (o *ConnectorHTTPVersion) SetSnapshot(v map[string]interface{})`

SetSnapshot sets Snapshot field to given value.

### HasSnapshot

`func (o *ConnectorHTTPVersion) HasSnapshot() bool`

HasSnapshot returns a boolean if a field has been set.

### SetSnapshotNil

`func (o *ConnectorHTTPVersion) SetSnapshotNil(b bool)`

 SetSnapshotNil sets the value for Snapshot to be an explicit nil

### UnsetSnapshot
`func (o *ConnectorHTTPVersion) UnsetSnapshot()`

UnsetSnapshot ensures that no value is present for Snapshot, not even an explicit nil
### GetCreatedAt

`func (o *ConnectorHTTPVersion) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *ConnectorHTTPVersion) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *ConnectorHTTPVersion) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *ConnectorHTTPVersion) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetReadyAt

`func (o *ConnectorHTTPVersion) GetReadyAt() time.Time`

GetReadyAt returns the ReadyAt field if non-nil, zero value otherwise.

### GetReadyAtOk

`func (o *ConnectorHTTPVersion) GetReadyAtOk() (*time.Time, bool)`

GetReadyAtOk returns a tuple with the ReadyAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadyAt

`func (o *ConnectorHTTPVersion) SetReadyAt(v time.Time)`

SetReadyAt sets ReadyAt field to given value.

### HasReadyAt

`func (o *ConnectorHTTPVersion) HasReadyAt() bool`

HasReadyAt returns a boolean if a field has been set.

### SetReadyAtNil

`func (o *ConnectorHTTPVersion) SetReadyAtNil(b bool)`

 SetReadyAtNil sets the value for ReadyAt to be an explicit nil

### UnsetReadyAt
`func (o *ConnectorHTTPVersion) UnsetReadyAt()`

UnsetReadyAt ensures that no value is present for ReadyAt, not even an explicit nil
### GetDescription

`func (o *ConnectorHTTPVersion) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *ConnectorHTTPVersion) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *ConnectorHTTPVersion) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *ConnectorHTTPVersion) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetBuildAt

`func (o *ConnectorHTTPVersion) GetBuildAt() time.Time`

GetBuildAt returns the BuildAt field if non-nil, zero value otherwise.

### GetBuildAtOk

`func (o *ConnectorHTTPVersion) GetBuildAtOk() (*time.Time, bool)`

GetBuildAtOk returns a tuple with the BuildAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildAt

`func (o *ConnectorHTTPVersion) SetBuildAt(v time.Time)`

SetBuildAt sets BuildAt field to given value.

### HasBuildAt

`func (o *ConnectorHTTPVersion) HasBuildAt() bool`

HasBuildAt returns a boolean if a field has been set.

### SetBuildAtNil

`func (o *ConnectorHTTPVersion) SetBuildAtNil(b bool)`

 SetBuildAtNil sets the value for BuildAt to be an explicit nil

### UnsetBuildAt
`func (o *ConnectorHTTPVersion) UnsetBuildAt()`

UnsetBuildAt ensures that no value is present for BuildAt, not even an explicit nil
### GetBuildComment

`func (o *ConnectorHTTPVersion) GetBuildComment() string`

GetBuildComment returns the BuildComment field if non-nil, zero value otherwise.

### GetBuildCommentOk

`func (o *ConnectorHTTPVersion) GetBuildCommentOk() (*string, bool)`

GetBuildCommentOk returns a tuple with the BuildComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildComment

`func (o *ConnectorHTTPVersion) SetBuildComment(v string)`

SetBuildComment sets BuildComment field to given value.

### HasBuildComment

`func (o *ConnectorHTTPVersion) HasBuildComment() bool`

HasBuildComment returns a boolean if a field has been set.

### GetCancelAt

`func (o *ConnectorHTTPVersion) GetCancelAt() time.Time`

GetCancelAt returns the CancelAt field if non-nil, zero value otherwise.

### GetCancelAtOk

`func (o *ConnectorHTTPVersion) GetCancelAtOk() (*time.Time, bool)`

GetCancelAtOk returns a tuple with the CancelAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelAt

`func (o *ConnectorHTTPVersion) SetCancelAt(v time.Time)`

SetCancelAt sets CancelAt field to given value.

### HasCancelAt

`func (o *ConnectorHTTPVersion) HasCancelAt() bool`

HasCancelAt returns a boolean if a field has been set.

### SetCancelAtNil

`func (o *ConnectorHTTPVersion) SetCancelAtNil(b bool)`

 SetCancelAtNil sets the value for CancelAt to be an explicit nil

### UnsetCancelAt
`func (o *ConnectorHTTPVersion) UnsetCancelAt()`

UnsetCancelAt ensures that no value is present for CancelAt, not even an explicit nil
### GetCancelComment

`func (o *ConnectorHTTPVersion) GetCancelComment() string`

GetCancelComment returns the CancelComment field if non-nil, zero value otherwise.

### GetCancelCommentOk

`func (o *ConnectorHTTPVersion) GetCancelCommentOk() (*string, bool)`

GetCancelCommentOk returns a tuple with the CancelComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelComment

`func (o *ConnectorHTTPVersion) SetCancelComment(v string)`

SetCancelComment sets CancelComment field to given value.

### HasCancelComment

`func (o *ConnectorHTTPVersion) HasCancelComment() bool`

HasCancelComment returns a boolean if a field has been set.

### GetArchivedAt

`func (o *ConnectorHTTPVersion) GetArchivedAt() time.Time`

GetArchivedAt returns the ArchivedAt field if non-nil, zero value otherwise.

### GetArchivedAtOk

`func (o *ConnectorHTTPVersion) GetArchivedAtOk() (*time.Time, bool)`

GetArchivedAtOk returns a tuple with the ArchivedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchivedAt

`func (o *ConnectorHTTPVersion) SetArchivedAt(v time.Time)`

SetArchivedAt sets ArchivedAt field to given value.

### HasArchivedAt

`func (o *ConnectorHTTPVersion) HasArchivedAt() bool`

HasArchivedAt returns a boolean if a field has been set.

### SetArchivedAtNil

`func (o *ConnectorHTTPVersion) SetArchivedAtNil(b bool)`

 SetArchivedAtNil sets the value for ArchivedAt to be an explicit nil

### UnsetArchivedAt
`func (o *ConnectorHTTPVersion) UnsetArchivedAt()`

UnsetArchivedAt ensures that no value is present for ArchivedAt, not even an explicit nil
### GetArchiveComment

`func (o *ConnectorHTTPVersion) GetArchiveComment() string`

GetArchiveComment returns the ArchiveComment field if non-nil, zero value otherwise.

### GetArchiveCommentOk

`func (o *ConnectorHTTPVersion) GetArchiveCommentOk() (*string, bool)`

GetArchiveCommentOk returns a tuple with the ArchiveComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchiveComment

`func (o *ConnectorHTTPVersion) SetArchiveComment(v string)`

SetArchiveComment sets ArchiveComment field to given value.

### HasArchiveComment

`func (o *ConnectorHTTPVersion) HasArchiveComment() bool`

HasArchiveComment returns a boolean if a field has been set.

### GetLastError

`func (o *ConnectorHTTPVersion) GetLastError() map[string]interface{}`

GetLastError returns the LastError field if non-nil, zero value otherwise.

### GetLastErrorOk

`func (o *ConnectorHTTPVersion) GetLastErrorOk() (*map[string]interface{}, bool)`

GetLastErrorOk returns a tuple with the LastError field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastError

`func (o *ConnectorHTTPVersion) SetLastError(v map[string]interface{})`

SetLastError sets LastError field to given value.

### HasLastError

`func (o *ConnectorHTTPVersion) HasLastError() bool`

HasLastError returns a boolean if a field has been set.

### SetLastErrorNil

`func (o *ConnectorHTTPVersion) SetLastErrorNil(b bool)`

 SetLastErrorNil sets the value for LastError to be an explicit nil

### UnsetLastError
`func (o *ConnectorHTTPVersion) UnsetLastError()`

UnsetLastError ensures that no value is present for LastError, not even an explicit nil
### GetTraceId

`func (o *ConnectorHTTPVersion) GetTraceId() string`

GetTraceId returns the TraceId field if non-nil, zero value otherwise.

### GetTraceIdOk

`func (o *ConnectorHTTPVersion) GetTraceIdOk() (*string, bool)`

GetTraceIdOk returns a tuple with the TraceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraceId

`func (o *ConnectorHTTPVersion) SetTraceId(v string)`

SetTraceId sets TraceId field to given value.

### HasTraceId

`func (o *ConnectorHTTPVersion) HasTraceId() bool`

HasTraceId returns a boolean if a field has been set.

### GetDependencies

`func (o *ConnectorHTTPVersion) GetDependencies() []map[string][]ApplicationVersionDependenciesInnerValueInner`

GetDependencies returns the Dependencies field if non-nil, zero value otherwise.

### GetDependenciesOk

`func (o *ConnectorHTTPVersion) GetDependenciesOk() (*[]map[string][]ApplicationVersionDependenciesInnerValueInner, bool)`

GetDependenciesOk returns a tuple with the Dependencies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDependencies

`func (o *ConnectorHTTPVersion) SetDependencies(v []map[string][]ApplicationVersionDependenciesInnerValueInner)`

SetDependencies sets Dependencies field to given value.

### HasDependencies

`func (o *ConnectorHTTPVersion) HasDependencies() bool`

HasDependencies returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


