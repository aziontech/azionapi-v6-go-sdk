# EnvironmentVersion

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**VersionId** | Pointer to **string** | ID of the version metadata. | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **NullableString** |  | [optional] 
**DeploymentPolicy** | Pointer to **string** | * &#x60;single_version&#x60; - single_version * &#x60;versioned_urls&#x60; - versioned_urls | [optional] 
**LogVerbosity** | Pointer to **string** | * &#x60;normal&#x60; - normal * &#x60;verbose&#x60; - verbose | [optional] 
**RobotsPolicy** | Pointer to **string** | * &#x60;index&#x60; - index * &#x60;noindex&#x60; - noindex * &#x60;respect_origin&#x60; - respect_origin | [optional] 
**Protection** | Pointer to [**EnvironmentProtection**](EnvironmentProtection.md) |  | [optional] 
**BranchTracking** | Pointer to [**NullableEnvironmentBranchTracking**](EnvironmentBranchTracking.md) |  | [optional] 
**VersionState** | Pointer to **string** | Current lifecycle state of the version.  * &#x60;draft&#x60; - draft * &#x60;queued&#x60; - queued * &#x60;building&#x60; - building * &#x60;ready&#x60; - ready * &#x60;error&#x60; - error * &#x60;canceled&#x60; - canceled * &#x60;archiving&#x60; - archiving * &#x60;archived&#x60; - archived * &#x60;deleting&#x60; - deleting * &#x60;deleted&#x60; - deleted | [optional] 
**ProductVersion** | Pointer to **NullableString** | Product version string. | [optional] 
**ClientId** | Pointer to **string** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** | When this version was created. | [optional] 
**LastModified** | Pointer to **NullableTime** |  | [optional] 
**CreatedBy** | Pointer to **NullableString** |  | [optional] 
**LastEditor** | Pointer to **NullableString** |  | [optional] 
**EnvironmentId** | Pointer to **string** |  | [optional] 
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

### NewEnvironmentVersion

`func NewEnvironmentVersion() *EnvironmentVersion`

NewEnvironmentVersion instantiates a new EnvironmentVersion object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEnvironmentVersionWithDefaults

`func NewEnvironmentVersionWithDefaults() *EnvironmentVersion`

NewEnvironmentVersionWithDefaults instantiates a new EnvironmentVersion object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersionId

`func (o *EnvironmentVersion) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *EnvironmentVersion) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *EnvironmentVersion) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *EnvironmentVersion) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### GetName

`func (o *EnvironmentVersion) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *EnvironmentVersion) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *EnvironmentVersion) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *EnvironmentVersion) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *EnvironmentVersion) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *EnvironmentVersion) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *EnvironmentVersion) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *EnvironmentVersion) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *EnvironmentVersion) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *EnvironmentVersion) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetDeploymentPolicy

`func (o *EnvironmentVersion) GetDeploymentPolicy() string`

GetDeploymentPolicy returns the DeploymentPolicy field if non-nil, zero value otherwise.

### GetDeploymentPolicyOk

`func (o *EnvironmentVersion) GetDeploymentPolicyOk() (*string, bool)`

GetDeploymentPolicyOk returns a tuple with the DeploymentPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentPolicy

`func (o *EnvironmentVersion) SetDeploymentPolicy(v string)`

SetDeploymentPolicy sets DeploymentPolicy field to given value.

### HasDeploymentPolicy

`func (o *EnvironmentVersion) HasDeploymentPolicy() bool`

HasDeploymentPolicy returns a boolean if a field has been set.

### GetLogVerbosity

`func (o *EnvironmentVersion) GetLogVerbosity() string`

GetLogVerbosity returns the LogVerbosity field if non-nil, zero value otherwise.

### GetLogVerbosityOk

`func (o *EnvironmentVersion) GetLogVerbosityOk() (*string, bool)`

GetLogVerbosityOk returns a tuple with the LogVerbosity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogVerbosity

`func (o *EnvironmentVersion) SetLogVerbosity(v string)`

SetLogVerbosity sets LogVerbosity field to given value.

### HasLogVerbosity

`func (o *EnvironmentVersion) HasLogVerbosity() bool`

HasLogVerbosity returns a boolean if a field has been set.

### GetRobotsPolicy

`func (o *EnvironmentVersion) GetRobotsPolicy() string`

GetRobotsPolicy returns the RobotsPolicy field if non-nil, zero value otherwise.

### GetRobotsPolicyOk

`func (o *EnvironmentVersion) GetRobotsPolicyOk() (*string, bool)`

GetRobotsPolicyOk returns a tuple with the RobotsPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRobotsPolicy

`func (o *EnvironmentVersion) SetRobotsPolicy(v string)`

SetRobotsPolicy sets RobotsPolicy field to given value.

### HasRobotsPolicy

`func (o *EnvironmentVersion) HasRobotsPolicy() bool`

HasRobotsPolicy returns a boolean if a field has been set.

### GetProtection

`func (o *EnvironmentVersion) GetProtection() EnvironmentProtection`

GetProtection returns the Protection field if non-nil, zero value otherwise.

### GetProtectionOk

`func (o *EnvironmentVersion) GetProtectionOk() (*EnvironmentProtection, bool)`

GetProtectionOk returns a tuple with the Protection field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProtection

`func (o *EnvironmentVersion) SetProtection(v EnvironmentProtection)`

SetProtection sets Protection field to given value.

### HasProtection

`func (o *EnvironmentVersion) HasProtection() bool`

HasProtection returns a boolean if a field has been set.

### GetBranchTracking

`func (o *EnvironmentVersion) GetBranchTracking() EnvironmentBranchTracking`

GetBranchTracking returns the BranchTracking field if non-nil, zero value otherwise.

### GetBranchTrackingOk

`func (o *EnvironmentVersion) GetBranchTrackingOk() (*EnvironmentBranchTracking, bool)`

GetBranchTrackingOk returns a tuple with the BranchTracking field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranchTracking

`func (o *EnvironmentVersion) SetBranchTracking(v EnvironmentBranchTracking)`

SetBranchTracking sets BranchTracking field to given value.

### HasBranchTracking

`func (o *EnvironmentVersion) HasBranchTracking() bool`

HasBranchTracking returns a boolean if a field has been set.

### SetBranchTrackingNil

`func (o *EnvironmentVersion) SetBranchTrackingNil(b bool)`

 SetBranchTrackingNil sets the value for BranchTracking to be an explicit nil

### UnsetBranchTracking
`func (o *EnvironmentVersion) UnsetBranchTracking()`

UnsetBranchTracking ensures that no value is present for BranchTracking, not even an explicit nil
### GetVersionState

`func (o *EnvironmentVersion) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *EnvironmentVersion) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *EnvironmentVersion) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *EnvironmentVersion) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetProductVersion

`func (o *EnvironmentVersion) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *EnvironmentVersion) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *EnvironmentVersion) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.

### HasProductVersion

`func (o *EnvironmentVersion) HasProductVersion() bool`

HasProductVersion returns a boolean if a field has been set.

### SetProductVersionNil

`func (o *EnvironmentVersion) SetProductVersionNil(b bool)`

 SetProductVersionNil sets the value for ProductVersion to be an explicit nil

### UnsetProductVersion
`func (o *EnvironmentVersion) UnsetProductVersion()`

UnsetProductVersion ensures that no value is present for ProductVersion, not even an explicit nil
### GetClientId

`func (o *EnvironmentVersion) GetClientId() string`

GetClientId returns the ClientId field if non-nil, zero value otherwise.

### GetClientIdOk

`func (o *EnvironmentVersion) GetClientIdOk() (*string, bool)`

GetClientIdOk returns a tuple with the ClientId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientId

`func (o *EnvironmentVersion) SetClientId(v string)`

SetClientId sets ClientId field to given value.

### HasClientId

`func (o *EnvironmentVersion) HasClientId() bool`

HasClientId returns a boolean if a field has been set.

### GetCreatedAt

`func (o *EnvironmentVersion) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *EnvironmentVersion) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *EnvironmentVersion) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *EnvironmentVersion) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetLastModified

`func (o *EnvironmentVersion) GetLastModified() time.Time`

GetLastModified returns the LastModified field if non-nil, zero value otherwise.

### GetLastModifiedOk

`func (o *EnvironmentVersion) GetLastModifiedOk() (*time.Time, bool)`

GetLastModifiedOk returns a tuple with the LastModified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastModified

`func (o *EnvironmentVersion) SetLastModified(v time.Time)`

SetLastModified sets LastModified field to given value.

### HasLastModified

`func (o *EnvironmentVersion) HasLastModified() bool`

HasLastModified returns a boolean if a field has been set.

### SetLastModifiedNil

`func (o *EnvironmentVersion) SetLastModifiedNil(b bool)`

 SetLastModifiedNil sets the value for LastModified to be an explicit nil

### UnsetLastModified
`func (o *EnvironmentVersion) UnsetLastModified()`

UnsetLastModified ensures that no value is present for LastModified, not even an explicit nil
### GetCreatedBy

`func (o *EnvironmentVersion) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *EnvironmentVersion) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *EnvironmentVersion) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.

### HasCreatedBy

`func (o *EnvironmentVersion) HasCreatedBy() bool`

HasCreatedBy returns a boolean if a field has been set.

### SetCreatedByNil

`func (o *EnvironmentVersion) SetCreatedByNil(b bool)`

 SetCreatedByNil sets the value for CreatedBy to be an explicit nil

### UnsetCreatedBy
`func (o *EnvironmentVersion) UnsetCreatedBy()`

UnsetCreatedBy ensures that no value is present for CreatedBy, not even an explicit nil
### GetLastEditor

`func (o *EnvironmentVersion) GetLastEditor() string`

GetLastEditor returns the LastEditor field if non-nil, zero value otherwise.

### GetLastEditorOk

`func (o *EnvironmentVersion) GetLastEditorOk() (*string, bool)`

GetLastEditorOk returns a tuple with the LastEditor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEditor

`func (o *EnvironmentVersion) SetLastEditor(v string)`

SetLastEditor sets LastEditor field to given value.

### HasLastEditor

`func (o *EnvironmentVersion) HasLastEditor() bool`

HasLastEditor returns a boolean if a field has been set.

### SetLastEditorNil

`func (o *EnvironmentVersion) SetLastEditorNil(b bool)`

 SetLastEditorNil sets the value for LastEditor to be an explicit nil

### UnsetLastEditor
`func (o *EnvironmentVersion) UnsetLastEditor()`

UnsetLastEditor ensures that no value is present for LastEditor, not even an explicit nil
### GetEnvironmentId

`func (o *EnvironmentVersion) GetEnvironmentId() string`

GetEnvironmentId returns the EnvironmentId field if non-nil, zero value otherwise.

### GetEnvironmentIdOk

`func (o *EnvironmentVersion) GetEnvironmentIdOk() (*string, bool)`

GetEnvironmentIdOk returns a tuple with the EnvironmentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnvironmentId

`func (o *EnvironmentVersion) SetEnvironmentId(v string)`

SetEnvironmentId sets EnvironmentId field to given value.

### HasEnvironmentId

`func (o *EnvironmentVersion) HasEnvironmentId() bool`

HasEnvironmentId returns a boolean if a field has been set.

### GetSourceVersionId

`func (o *EnvironmentVersion) GetSourceVersionId() string`

GetSourceVersionId returns the SourceVersionId field if non-nil, zero value otherwise.

### GetSourceVersionIdOk

`func (o *EnvironmentVersion) GetSourceVersionIdOk() (*string, bool)`

GetSourceVersionIdOk returns a tuple with the SourceVersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceVersionId

`func (o *EnvironmentVersion) SetSourceVersionId(v string)`

SetSourceVersionId sets SourceVersionId field to given value.

### HasSourceVersionId

`func (o *EnvironmentVersion) HasSourceVersionId() bool`

HasSourceVersionId returns a boolean if a field has been set.

### SetSourceVersionIdNil

`func (o *EnvironmentVersion) SetSourceVersionIdNil(b bool)`

 SetSourceVersionIdNil sets the value for SourceVersionId to be an explicit nil

### UnsetSourceVersionId
`func (o *EnvironmentVersion) UnsetSourceVersionId()`

UnsetSourceVersionId ensures that no value is present for SourceVersionId, not even an explicit nil
### GetSnapshot

`func (o *EnvironmentVersion) GetSnapshot() map[string]interface{}`

GetSnapshot returns the Snapshot field if non-nil, zero value otherwise.

### GetSnapshotOk

`func (o *EnvironmentVersion) GetSnapshotOk() (*map[string]interface{}, bool)`

GetSnapshotOk returns a tuple with the Snapshot field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnapshot

`func (o *EnvironmentVersion) SetSnapshot(v map[string]interface{})`

SetSnapshot sets Snapshot field to given value.

### HasSnapshot

`func (o *EnvironmentVersion) HasSnapshot() bool`

HasSnapshot returns a boolean if a field has been set.

### SetSnapshotNil

`func (o *EnvironmentVersion) SetSnapshotNil(b bool)`

 SetSnapshotNil sets the value for Snapshot to be an explicit nil

### UnsetSnapshot
`func (o *EnvironmentVersion) UnsetSnapshot()`

UnsetSnapshot ensures that no value is present for Snapshot, not even an explicit nil
### GetReadyAt

`func (o *EnvironmentVersion) GetReadyAt() time.Time`

GetReadyAt returns the ReadyAt field if non-nil, zero value otherwise.

### GetReadyAtOk

`func (o *EnvironmentVersion) GetReadyAtOk() (*time.Time, bool)`

GetReadyAtOk returns a tuple with the ReadyAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadyAt

`func (o *EnvironmentVersion) SetReadyAt(v time.Time)`

SetReadyAt sets ReadyAt field to given value.

### HasReadyAt

`func (o *EnvironmentVersion) HasReadyAt() bool`

HasReadyAt returns a boolean if a field has been set.

### SetReadyAtNil

`func (o *EnvironmentVersion) SetReadyAtNil(b bool)`

 SetReadyAtNil sets the value for ReadyAt to be an explicit nil

### UnsetReadyAt
`func (o *EnvironmentVersion) UnsetReadyAt()`

UnsetReadyAt ensures that no value is present for ReadyAt, not even an explicit nil
### GetBuildAt

`func (o *EnvironmentVersion) GetBuildAt() time.Time`

GetBuildAt returns the BuildAt field if non-nil, zero value otherwise.

### GetBuildAtOk

`func (o *EnvironmentVersion) GetBuildAtOk() (*time.Time, bool)`

GetBuildAtOk returns a tuple with the BuildAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildAt

`func (o *EnvironmentVersion) SetBuildAt(v time.Time)`

SetBuildAt sets BuildAt field to given value.

### HasBuildAt

`func (o *EnvironmentVersion) HasBuildAt() bool`

HasBuildAt returns a boolean if a field has been set.

### SetBuildAtNil

`func (o *EnvironmentVersion) SetBuildAtNil(b bool)`

 SetBuildAtNil sets the value for BuildAt to be an explicit nil

### UnsetBuildAt
`func (o *EnvironmentVersion) UnsetBuildAt()`

UnsetBuildAt ensures that no value is present for BuildAt, not even an explicit nil
### GetBuildComment

`func (o *EnvironmentVersion) GetBuildComment() string`

GetBuildComment returns the BuildComment field if non-nil, zero value otherwise.

### GetBuildCommentOk

`func (o *EnvironmentVersion) GetBuildCommentOk() (*string, bool)`

GetBuildCommentOk returns a tuple with the BuildComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildComment

`func (o *EnvironmentVersion) SetBuildComment(v string)`

SetBuildComment sets BuildComment field to given value.

### HasBuildComment

`func (o *EnvironmentVersion) HasBuildComment() bool`

HasBuildComment returns a boolean if a field has been set.

### SetBuildCommentNil

`func (o *EnvironmentVersion) SetBuildCommentNil(b bool)`

 SetBuildCommentNil sets the value for BuildComment to be an explicit nil

### UnsetBuildComment
`func (o *EnvironmentVersion) UnsetBuildComment()`

UnsetBuildComment ensures that no value is present for BuildComment, not even an explicit nil
### GetCancelAt

`func (o *EnvironmentVersion) GetCancelAt() time.Time`

GetCancelAt returns the CancelAt field if non-nil, zero value otherwise.

### GetCancelAtOk

`func (o *EnvironmentVersion) GetCancelAtOk() (*time.Time, bool)`

GetCancelAtOk returns a tuple with the CancelAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelAt

`func (o *EnvironmentVersion) SetCancelAt(v time.Time)`

SetCancelAt sets CancelAt field to given value.

### HasCancelAt

`func (o *EnvironmentVersion) HasCancelAt() bool`

HasCancelAt returns a boolean if a field has been set.

### SetCancelAtNil

`func (o *EnvironmentVersion) SetCancelAtNil(b bool)`

 SetCancelAtNil sets the value for CancelAt to be an explicit nil

### UnsetCancelAt
`func (o *EnvironmentVersion) UnsetCancelAt()`

UnsetCancelAt ensures that no value is present for CancelAt, not even an explicit nil
### GetCancelComment

`func (o *EnvironmentVersion) GetCancelComment() string`

GetCancelComment returns the CancelComment field if non-nil, zero value otherwise.

### GetCancelCommentOk

`func (o *EnvironmentVersion) GetCancelCommentOk() (*string, bool)`

GetCancelCommentOk returns a tuple with the CancelComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelComment

`func (o *EnvironmentVersion) SetCancelComment(v string)`

SetCancelComment sets CancelComment field to given value.

### HasCancelComment

`func (o *EnvironmentVersion) HasCancelComment() bool`

HasCancelComment returns a boolean if a field has been set.

### SetCancelCommentNil

`func (o *EnvironmentVersion) SetCancelCommentNil(b bool)`

 SetCancelCommentNil sets the value for CancelComment to be an explicit nil

### UnsetCancelComment
`func (o *EnvironmentVersion) UnsetCancelComment()`

UnsetCancelComment ensures that no value is present for CancelComment, not even an explicit nil
### GetArchivedAt

`func (o *EnvironmentVersion) GetArchivedAt() time.Time`

GetArchivedAt returns the ArchivedAt field if non-nil, zero value otherwise.

### GetArchivedAtOk

`func (o *EnvironmentVersion) GetArchivedAtOk() (*time.Time, bool)`

GetArchivedAtOk returns a tuple with the ArchivedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchivedAt

`func (o *EnvironmentVersion) SetArchivedAt(v time.Time)`

SetArchivedAt sets ArchivedAt field to given value.

### HasArchivedAt

`func (o *EnvironmentVersion) HasArchivedAt() bool`

HasArchivedAt returns a boolean if a field has been set.

### SetArchivedAtNil

`func (o *EnvironmentVersion) SetArchivedAtNil(b bool)`

 SetArchivedAtNil sets the value for ArchivedAt to be an explicit nil

### UnsetArchivedAt
`func (o *EnvironmentVersion) UnsetArchivedAt()`

UnsetArchivedAt ensures that no value is present for ArchivedAt, not even an explicit nil
### GetArchiveComment

`func (o *EnvironmentVersion) GetArchiveComment() string`

GetArchiveComment returns the ArchiveComment field if non-nil, zero value otherwise.

### GetArchiveCommentOk

`func (o *EnvironmentVersion) GetArchiveCommentOk() (*string, bool)`

GetArchiveCommentOk returns a tuple with the ArchiveComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchiveComment

`func (o *EnvironmentVersion) SetArchiveComment(v string)`

SetArchiveComment sets ArchiveComment field to given value.

### HasArchiveComment

`func (o *EnvironmentVersion) HasArchiveComment() bool`

HasArchiveComment returns a boolean if a field has been set.

### SetArchiveCommentNil

`func (o *EnvironmentVersion) SetArchiveCommentNil(b bool)`

 SetArchiveCommentNil sets the value for ArchiveComment to be an explicit nil

### UnsetArchiveComment
`func (o *EnvironmentVersion) UnsetArchiveComment()`

UnsetArchiveComment ensures that no value is present for ArchiveComment, not even an explicit nil
### GetLastError

`func (o *EnvironmentVersion) GetLastError() map[string]interface{}`

GetLastError returns the LastError field if non-nil, zero value otherwise.

### GetLastErrorOk

`func (o *EnvironmentVersion) GetLastErrorOk() (*map[string]interface{}, bool)`

GetLastErrorOk returns a tuple with the LastError field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastError

`func (o *EnvironmentVersion) SetLastError(v map[string]interface{})`

SetLastError sets LastError field to given value.

### HasLastError

`func (o *EnvironmentVersion) HasLastError() bool`

HasLastError returns a boolean if a field has been set.

### SetLastErrorNil

`func (o *EnvironmentVersion) SetLastErrorNil(b bool)`

 SetLastErrorNil sets the value for LastError to be an explicit nil

### UnsetLastError
`func (o *EnvironmentVersion) UnsetLastError()`

UnsetLastError ensures that no value is present for LastError, not even an explicit nil
### GetTraceId

`func (o *EnvironmentVersion) GetTraceId() string`

GetTraceId returns the TraceId field if non-nil, zero value otherwise.

### GetTraceIdOk

`func (o *EnvironmentVersion) GetTraceIdOk() (*string, bool)`

GetTraceIdOk returns a tuple with the TraceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraceId

`func (o *EnvironmentVersion) SetTraceId(v string)`

SetTraceId sets TraceId field to given value.

### HasTraceId

`func (o *EnvironmentVersion) HasTraceId() bool`

HasTraceId returns a boolean if a field has been set.

### SetTraceIdNil

`func (o *EnvironmentVersion) SetTraceIdNil(b bool)`

 SetTraceIdNil sets the value for TraceId to be an explicit nil

### UnsetTraceId
`func (o *EnvironmentVersion) UnsetTraceId()`

UnsetTraceId ensures that no value is present for TraceId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


