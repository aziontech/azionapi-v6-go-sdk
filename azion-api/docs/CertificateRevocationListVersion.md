# CertificateRevocationListVersion

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**LastEditor** | Pointer to **string** |  | [optional] 
**LastModified** | Pointer to **time.Time** | Timestamp of the last modification made to the certificate content on the platform. | [optional] 
**Issuer** | Pointer to **string** |  | [optional] 
**LastUpdate** | Pointer to **time.Time** | Timestamp of the last update issued by the certification revocation list issuer. | [optional] 
**NextUpdate** | Pointer to **time.Time** | Timestamp of the next scheduled update from the certification revocation list issuer. | [optional] 
**Crl** | Pointer to **string** |  | [optional] 
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

### NewCertificateRevocationListVersion

`func NewCertificateRevocationListVersion() *CertificateRevocationListVersion`

NewCertificateRevocationListVersion instantiates a new CertificateRevocationListVersion object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCertificateRevocationListVersionWithDefaults

`func NewCertificateRevocationListVersionWithDefaults() *CertificateRevocationListVersion`

NewCertificateRevocationListVersionWithDefaults instantiates a new CertificateRevocationListVersion object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CertificateRevocationListVersion) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CertificateRevocationListVersion) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CertificateRevocationListVersion) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *CertificateRevocationListVersion) HasName() bool`

HasName returns a boolean if a field has been set.

### GetLastEditor

`func (o *CertificateRevocationListVersion) GetLastEditor() string`

GetLastEditor returns the LastEditor field if non-nil, zero value otherwise.

### GetLastEditorOk

`func (o *CertificateRevocationListVersion) GetLastEditorOk() (*string, bool)`

GetLastEditorOk returns a tuple with the LastEditor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEditor

`func (o *CertificateRevocationListVersion) SetLastEditor(v string)`

SetLastEditor sets LastEditor field to given value.

### HasLastEditor

`func (o *CertificateRevocationListVersion) HasLastEditor() bool`

HasLastEditor returns a boolean if a field has been set.

### GetLastModified

`func (o *CertificateRevocationListVersion) GetLastModified() time.Time`

GetLastModified returns the LastModified field if non-nil, zero value otherwise.

### GetLastModifiedOk

`func (o *CertificateRevocationListVersion) GetLastModifiedOk() (*time.Time, bool)`

GetLastModifiedOk returns a tuple with the LastModified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastModified

`func (o *CertificateRevocationListVersion) SetLastModified(v time.Time)`

SetLastModified sets LastModified field to given value.

### HasLastModified

`func (o *CertificateRevocationListVersion) HasLastModified() bool`

HasLastModified returns a boolean if a field has been set.

### GetIssuer

`func (o *CertificateRevocationListVersion) GetIssuer() string`

GetIssuer returns the Issuer field if non-nil, zero value otherwise.

### GetIssuerOk

`func (o *CertificateRevocationListVersion) GetIssuerOk() (*string, bool)`

GetIssuerOk returns a tuple with the Issuer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssuer

`func (o *CertificateRevocationListVersion) SetIssuer(v string)`

SetIssuer sets Issuer field to given value.

### HasIssuer

`func (o *CertificateRevocationListVersion) HasIssuer() bool`

HasIssuer returns a boolean if a field has been set.

### GetLastUpdate

`func (o *CertificateRevocationListVersion) GetLastUpdate() time.Time`

GetLastUpdate returns the LastUpdate field if non-nil, zero value otherwise.

### GetLastUpdateOk

`func (o *CertificateRevocationListVersion) GetLastUpdateOk() (*time.Time, bool)`

GetLastUpdateOk returns a tuple with the LastUpdate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastUpdate

`func (o *CertificateRevocationListVersion) SetLastUpdate(v time.Time)`

SetLastUpdate sets LastUpdate field to given value.

### HasLastUpdate

`func (o *CertificateRevocationListVersion) HasLastUpdate() bool`

HasLastUpdate returns a boolean if a field has been set.

### GetNextUpdate

`func (o *CertificateRevocationListVersion) GetNextUpdate() time.Time`

GetNextUpdate returns the NextUpdate field if non-nil, zero value otherwise.

### GetNextUpdateOk

`func (o *CertificateRevocationListVersion) GetNextUpdateOk() (*time.Time, bool)`

GetNextUpdateOk returns a tuple with the NextUpdate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextUpdate

`func (o *CertificateRevocationListVersion) SetNextUpdate(v time.Time)`

SetNextUpdate sets NextUpdate field to given value.

### HasNextUpdate

`func (o *CertificateRevocationListVersion) HasNextUpdate() bool`

HasNextUpdate returns a boolean if a field has been set.

### GetCrl

`func (o *CertificateRevocationListVersion) GetCrl() string`

GetCrl returns the Crl field if non-nil, zero value otherwise.

### GetCrlOk

`func (o *CertificateRevocationListVersion) GetCrlOk() (*string, bool)`

GetCrlOk returns a tuple with the Crl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCrl

`func (o *CertificateRevocationListVersion) SetCrl(v string)`

SetCrl sets Crl field to given value.

### HasCrl

`func (o *CertificateRevocationListVersion) HasCrl() bool`

HasCrl returns a boolean if a field has been set.

### GetVersionId

`func (o *CertificateRevocationListVersion) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *CertificateRevocationListVersion) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *CertificateRevocationListVersion) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *CertificateRevocationListVersion) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### GetVersionState

`func (o *CertificateRevocationListVersion) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *CertificateRevocationListVersion) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *CertificateRevocationListVersion) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *CertificateRevocationListVersion) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetProductVersion

`func (o *CertificateRevocationListVersion) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *CertificateRevocationListVersion) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *CertificateRevocationListVersion) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.

### HasProductVersion

`func (o *CertificateRevocationListVersion) HasProductVersion() bool`

HasProductVersion returns a boolean if a field has been set.

### GetSourceVersionId

`func (o *CertificateRevocationListVersion) GetSourceVersionId() string`

GetSourceVersionId returns the SourceVersionId field if non-nil, zero value otherwise.

### GetSourceVersionIdOk

`func (o *CertificateRevocationListVersion) GetSourceVersionIdOk() (*string, bool)`

GetSourceVersionIdOk returns a tuple with the SourceVersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceVersionId

`func (o *CertificateRevocationListVersion) SetSourceVersionId(v string)`

SetSourceVersionId sets SourceVersionId field to given value.

### HasSourceVersionId

`func (o *CertificateRevocationListVersion) HasSourceVersionId() bool`

HasSourceVersionId returns a boolean if a field has been set.

### SetSourceVersionIdNil

`func (o *CertificateRevocationListVersion) SetSourceVersionIdNil(b bool)`

 SetSourceVersionIdNil sets the value for SourceVersionId to be an explicit nil

### UnsetSourceVersionId
`func (o *CertificateRevocationListVersion) UnsetSourceVersionId()`

UnsetSourceVersionId ensures that no value is present for SourceVersionId, not even an explicit nil
### GetSnapshot

`func (o *CertificateRevocationListVersion) GetSnapshot() map[string]interface{}`

GetSnapshot returns the Snapshot field if non-nil, zero value otherwise.

### GetSnapshotOk

`func (o *CertificateRevocationListVersion) GetSnapshotOk() (*map[string]interface{}, bool)`

GetSnapshotOk returns a tuple with the Snapshot field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnapshot

`func (o *CertificateRevocationListVersion) SetSnapshot(v map[string]interface{})`

SetSnapshot sets Snapshot field to given value.

### HasSnapshot

`func (o *CertificateRevocationListVersion) HasSnapshot() bool`

HasSnapshot returns a boolean if a field has been set.

### SetSnapshotNil

`func (o *CertificateRevocationListVersion) SetSnapshotNil(b bool)`

 SetSnapshotNil sets the value for Snapshot to be an explicit nil

### UnsetSnapshot
`func (o *CertificateRevocationListVersion) UnsetSnapshot()`

UnsetSnapshot ensures that no value is present for Snapshot, not even an explicit nil
### GetCreatedAt

`func (o *CertificateRevocationListVersion) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *CertificateRevocationListVersion) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *CertificateRevocationListVersion) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *CertificateRevocationListVersion) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetReadyAt

`func (o *CertificateRevocationListVersion) GetReadyAt() time.Time`

GetReadyAt returns the ReadyAt field if non-nil, zero value otherwise.

### GetReadyAtOk

`func (o *CertificateRevocationListVersion) GetReadyAtOk() (*time.Time, bool)`

GetReadyAtOk returns a tuple with the ReadyAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadyAt

`func (o *CertificateRevocationListVersion) SetReadyAt(v time.Time)`

SetReadyAt sets ReadyAt field to given value.

### HasReadyAt

`func (o *CertificateRevocationListVersion) HasReadyAt() bool`

HasReadyAt returns a boolean if a field has been set.

### SetReadyAtNil

`func (o *CertificateRevocationListVersion) SetReadyAtNil(b bool)`

 SetReadyAtNil sets the value for ReadyAt to be an explicit nil

### UnsetReadyAt
`func (o *CertificateRevocationListVersion) UnsetReadyAt()`

UnsetReadyAt ensures that no value is present for ReadyAt, not even an explicit nil
### GetDescription

`func (o *CertificateRevocationListVersion) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CertificateRevocationListVersion) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CertificateRevocationListVersion) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CertificateRevocationListVersion) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetBuildAt

`func (o *CertificateRevocationListVersion) GetBuildAt() time.Time`

GetBuildAt returns the BuildAt field if non-nil, zero value otherwise.

### GetBuildAtOk

`func (o *CertificateRevocationListVersion) GetBuildAtOk() (*time.Time, bool)`

GetBuildAtOk returns a tuple with the BuildAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildAt

`func (o *CertificateRevocationListVersion) SetBuildAt(v time.Time)`

SetBuildAt sets BuildAt field to given value.

### HasBuildAt

`func (o *CertificateRevocationListVersion) HasBuildAt() bool`

HasBuildAt returns a boolean if a field has been set.

### SetBuildAtNil

`func (o *CertificateRevocationListVersion) SetBuildAtNil(b bool)`

 SetBuildAtNil sets the value for BuildAt to be an explicit nil

### UnsetBuildAt
`func (o *CertificateRevocationListVersion) UnsetBuildAt()`

UnsetBuildAt ensures that no value is present for BuildAt, not even an explicit nil
### GetBuildComment

`func (o *CertificateRevocationListVersion) GetBuildComment() string`

GetBuildComment returns the BuildComment field if non-nil, zero value otherwise.

### GetBuildCommentOk

`func (o *CertificateRevocationListVersion) GetBuildCommentOk() (*string, bool)`

GetBuildCommentOk returns a tuple with the BuildComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildComment

`func (o *CertificateRevocationListVersion) SetBuildComment(v string)`

SetBuildComment sets BuildComment field to given value.

### HasBuildComment

`func (o *CertificateRevocationListVersion) HasBuildComment() bool`

HasBuildComment returns a boolean if a field has been set.

### GetCancelAt

`func (o *CertificateRevocationListVersion) GetCancelAt() time.Time`

GetCancelAt returns the CancelAt field if non-nil, zero value otherwise.

### GetCancelAtOk

`func (o *CertificateRevocationListVersion) GetCancelAtOk() (*time.Time, bool)`

GetCancelAtOk returns a tuple with the CancelAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelAt

`func (o *CertificateRevocationListVersion) SetCancelAt(v time.Time)`

SetCancelAt sets CancelAt field to given value.

### HasCancelAt

`func (o *CertificateRevocationListVersion) HasCancelAt() bool`

HasCancelAt returns a boolean if a field has been set.

### SetCancelAtNil

`func (o *CertificateRevocationListVersion) SetCancelAtNil(b bool)`

 SetCancelAtNil sets the value for CancelAt to be an explicit nil

### UnsetCancelAt
`func (o *CertificateRevocationListVersion) UnsetCancelAt()`

UnsetCancelAt ensures that no value is present for CancelAt, not even an explicit nil
### GetCancelComment

`func (o *CertificateRevocationListVersion) GetCancelComment() string`

GetCancelComment returns the CancelComment field if non-nil, zero value otherwise.

### GetCancelCommentOk

`func (o *CertificateRevocationListVersion) GetCancelCommentOk() (*string, bool)`

GetCancelCommentOk returns a tuple with the CancelComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelComment

`func (o *CertificateRevocationListVersion) SetCancelComment(v string)`

SetCancelComment sets CancelComment field to given value.

### HasCancelComment

`func (o *CertificateRevocationListVersion) HasCancelComment() bool`

HasCancelComment returns a boolean if a field has been set.

### GetArchivedAt

`func (o *CertificateRevocationListVersion) GetArchivedAt() time.Time`

GetArchivedAt returns the ArchivedAt field if non-nil, zero value otherwise.

### GetArchivedAtOk

`func (o *CertificateRevocationListVersion) GetArchivedAtOk() (*time.Time, bool)`

GetArchivedAtOk returns a tuple with the ArchivedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchivedAt

`func (o *CertificateRevocationListVersion) SetArchivedAt(v time.Time)`

SetArchivedAt sets ArchivedAt field to given value.

### HasArchivedAt

`func (o *CertificateRevocationListVersion) HasArchivedAt() bool`

HasArchivedAt returns a boolean if a field has been set.

### SetArchivedAtNil

`func (o *CertificateRevocationListVersion) SetArchivedAtNil(b bool)`

 SetArchivedAtNil sets the value for ArchivedAt to be an explicit nil

### UnsetArchivedAt
`func (o *CertificateRevocationListVersion) UnsetArchivedAt()`

UnsetArchivedAt ensures that no value is present for ArchivedAt, not even an explicit nil
### GetArchiveComment

`func (o *CertificateRevocationListVersion) GetArchiveComment() string`

GetArchiveComment returns the ArchiveComment field if non-nil, zero value otherwise.

### GetArchiveCommentOk

`func (o *CertificateRevocationListVersion) GetArchiveCommentOk() (*string, bool)`

GetArchiveCommentOk returns a tuple with the ArchiveComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchiveComment

`func (o *CertificateRevocationListVersion) SetArchiveComment(v string)`

SetArchiveComment sets ArchiveComment field to given value.

### HasArchiveComment

`func (o *CertificateRevocationListVersion) HasArchiveComment() bool`

HasArchiveComment returns a boolean if a field has been set.

### GetLastError

`func (o *CertificateRevocationListVersion) GetLastError() map[string]interface{}`

GetLastError returns the LastError field if non-nil, zero value otherwise.

### GetLastErrorOk

`func (o *CertificateRevocationListVersion) GetLastErrorOk() (*map[string]interface{}, bool)`

GetLastErrorOk returns a tuple with the LastError field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastError

`func (o *CertificateRevocationListVersion) SetLastError(v map[string]interface{})`

SetLastError sets LastError field to given value.

### HasLastError

`func (o *CertificateRevocationListVersion) HasLastError() bool`

HasLastError returns a boolean if a field has been set.

### SetLastErrorNil

`func (o *CertificateRevocationListVersion) SetLastErrorNil(b bool)`

 SetLastErrorNil sets the value for LastError to be an explicit nil

### UnsetLastError
`func (o *CertificateRevocationListVersion) UnsetLastError()`

UnsetLastError ensures that no value is present for LastError, not even an explicit nil
### GetTraceId

`func (o *CertificateRevocationListVersion) GetTraceId() string`

GetTraceId returns the TraceId field if non-nil, zero value otherwise.

### GetTraceIdOk

`func (o *CertificateRevocationListVersion) GetTraceIdOk() (*string, bool)`

GetTraceIdOk returns a tuple with the TraceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraceId

`func (o *CertificateRevocationListVersion) SetTraceId(v string)`

SetTraceId sets TraceId field to given value.

### HasTraceId

`func (o *CertificateRevocationListVersion) HasTraceId() bool`

HasTraceId returns a boolean if a field has been set.

### GetDependencies

`func (o *CertificateRevocationListVersion) GetDependencies() []map[string][]ApplicationVersionDependenciesInnerValueInner`

GetDependencies returns the Dependencies field if non-nil, zero value otherwise.

### GetDependenciesOk

`func (o *CertificateRevocationListVersion) GetDependenciesOk() (*[]map[string][]ApplicationVersionDependenciesInnerValueInner, bool)`

GetDependenciesOk returns a tuple with the Dependencies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDependencies

`func (o *CertificateRevocationListVersion) SetDependencies(v []map[string][]ApplicationVersionDependenciesInnerValueInner)`

SetDependencies sets Dependencies field to given value.

### HasDependencies

`func (o *CertificateRevocationListVersion) HasDependencies() bool`

HasDependencies returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


