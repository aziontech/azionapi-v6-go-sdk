# CertificateVersion

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Certificate** | Pointer to **NullableString** |  | [optional] 
**PrivateKey** | Pointer to **NullableString** |  | [optional] 
**Issuer** | Pointer to **NullableString** |  | [optional] 
**SubjectName** | Pointer to **[]string** |  | [optional] 
**Validity** | Pointer to **NullableString** |  | [optional] 
**Type** | Pointer to **string** | The value can&#39;t be changed after the certificate creation.  * &#x60;edge_certificate&#x60; - Certificate * &#x60;trusted_ca_certificate&#x60; - Trusted CA Certificate | [optional] 
**Managed** | Pointer to **bool** |  | [optional] 
**Csr** | Pointer to **NullableString** |  | [optional] 
**Challenge** | Pointer to **string** |  | [optional] 
**Authority** | Pointer to **string** |  | [optional] 
**KeyAlgorithm** | Pointer to **string** |  | [optional] 
**LastEditor** | Pointer to **string** |  | [optional] 
**LastModified** | Pointer to **time.Time** | Timestamp of the last modification made to the certificate content on the platform. | [optional] 
**RenewedAt** | Pointer to **NullableTime** | Timestamp indicating when the managed certificate was renewed on our platform. | [optional] 
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

### NewCertificateVersion

`func NewCertificateVersion() *CertificateVersion`

NewCertificateVersion instantiates a new CertificateVersion object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCertificateVersionWithDefaults

`func NewCertificateVersionWithDefaults() *CertificateVersion`

NewCertificateVersionWithDefaults instantiates a new CertificateVersion object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CertificateVersion) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CertificateVersion) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CertificateVersion) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *CertificateVersion) HasName() bool`

HasName returns a boolean if a field has been set.

### GetCertificate

`func (o *CertificateVersion) GetCertificate() string`

GetCertificate returns the Certificate field if non-nil, zero value otherwise.

### GetCertificateOk

`func (o *CertificateVersion) GetCertificateOk() (*string, bool)`

GetCertificateOk returns a tuple with the Certificate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCertificate

`func (o *CertificateVersion) SetCertificate(v string)`

SetCertificate sets Certificate field to given value.

### HasCertificate

`func (o *CertificateVersion) HasCertificate() bool`

HasCertificate returns a boolean if a field has been set.

### SetCertificateNil

`func (o *CertificateVersion) SetCertificateNil(b bool)`

 SetCertificateNil sets the value for Certificate to be an explicit nil

### UnsetCertificate
`func (o *CertificateVersion) UnsetCertificate()`

UnsetCertificate ensures that no value is present for Certificate, not even an explicit nil
### GetPrivateKey

`func (o *CertificateVersion) GetPrivateKey() string`

GetPrivateKey returns the PrivateKey field if non-nil, zero value otherwise.

### GetPrivateKeyOk

`func (o *CertificateVersion) GetPrivateKeyOk() (*string, bool)`

GetPrivateKeyOk returns a tuple with the PrivateKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrivateKey

`func (o *CertificateVersion) SetPrivateKey(v string)`

SetPrivateKey sets PrivateKey field to given value.

### HasPrivateKey

`func (o *CertificateVersion) HasPrivateKey() bool`

HasPrivateKey returns a boolean if a field has been set.

### SetPrivateKeyNil

`func (o *CertificateVersion) SetPrivateKeyNil(b bool)`

 SetPrivateKeyNil sets the value for PrivateKey to be an explicit nil

### UnsetPrivateKey
`func (o *CertificateVersion) UnsetPrivateKey()`

UnsetPrivateKey ensures that no value is present for PrivateKey, not even an explicit nil
### GetIssuer

`func (o *CertificateVersion) GetIssuer() string`

GetIssuer returns the Issuer field if non-nil, zero value otherwise.

### GetIssuerOk

`func (o *CertificateVersion) GetIssuerOk() (*string, bool)`

GetIssuerOk returns a tuple with the Issuer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssuer

`func (o *CertificateVersion) SetIssuer(v string)`

SetIssuer sets Issuer field to given value.

### HasIssuer

`func (o *CertificateVersion) HasIssuer() bool`

HasIssuer returns a boolean if a field has been set.

### SetIssuerNil

`func (o *CertificateVersion) SetIssuerNil(b bool)`

 SetIssuerNil sets the value for Issuer to be an explicit nil

### UnsetIssuer
`func (o *CertificateVersion) UnsetIssuer()`

UnsetIssuer ensures that no value is present for Issuer, not even an explicit nil
### GetSubjectName

`func (o *CertificateVersion) GetSubjectName() []string`

GetSubjectName returns the SubjectName field if non-nil, zero value otherwise.

### GetSubjectNameOk

`func (o *CertificateVersion) GetSubjectNameOk() (*[]string, bool)`

GetSubjectNameOk returns a tuple with the SubjectName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubjectName

`func (o *CertificateVersion) SetSubjectName(v []string)`

SetSubjectName sets SubjectName field to given value.

### HasSubjectName

`func (o *CertificateVersion) HasSubjectName() bool`

HasSubjectName returns a boolean if a field has been set.

### GetValidity

`func (o *CertificateVersion) GetValidity() string`

GetValidity returns the Validity field if non-nil, zero value otherwise.

### GetValidityOk

`func (o *CertificateVersion) GetValidityOk() (*string, bool)`

GetValidityOk returns a tuple with the Validity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValidity

`func (o *CertificateVersion) SetValidity(v string)`

SetValidity sets Validity field to given value.

### HasValidity

`func (o *CertificateVersion) HasValidity() bool`

HasValidity returns a boolean if a field has been set.

### SetValidityNil

`func (o *CertificateVersion) SetValidityNil(b bool)`

 SetValidityNil sets the value for Validity to be an explicit nil

### UnsetValidity
`func (o *CertificateVersion) UnsetValidity()`

UnsetValidity ensures that no value is present for Validity, not even an explicit nil
### GetType

`func (o *CertificateVersion) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CertificateVersion) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CertificateVersion) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *CertificateVersion) HasType() bool`

HasType returns a boolean if a field has been set.

### GetManaged

`func (o *CertificateVersion) GetManaged() bool`

GetManaged returns the Managed field if non-nil, zero value otherwise.

### GetManagedOk

`func (o *CertificateVersion) GetManagedOk() (*bool, bool)`

GetManagedOk returns a tuple with the Managed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetManaged

`func (o *CertificateVersion) SetManaged(v bool)`

SetManaged sets Managed field to given value.

### HasManaged

`func (o *CertificateVersion) HasManaged() bool`

HasManaged returns a boolean if a field has been set.

### GetCsr

`func (o *CertificateVersion) GetCsr() string`

GetCsr returns the Csr field if non-nil, zero value otherwise.

### GetCsrOk

`func (o *CertificateVersion) GetCsrOk() (*string, bool)`

GetCsrOk returns a tuple with the Csr field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCsr

`func (o *CertificateVersion) SetCsr(v string)`

SetCsr sets Csr field to given value.

### HasCsr

`func (o *CertificateVersion) HasCsr() bool`

HasCsr returns a boolean if a field has been set.

### SetCsrNil

`func (o *CertificateVersion) SetCsrNil(b bool)`

 SetCsrNil sets the value for Csr to be an explicit nil

### UnsetCsr
`func (o *CertificateVersion) UnsetCsr()`

UnsetCsr ensures that no value is present for Csr, not even an explicit nil
### GetChallenge

`func (o *CertificateVersion) GetChallenge() string`

GetChallenge returns the Challenge field if non-nil, zero value otherwise.

### GetChallengeOk

`func (o *CertificateVersion) GetChallengeOk() (*string, bool)`

GetChallengeOk returns a tuple with the Challenge field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChallenge

`func (o *CertificateVersion) SetChallenge(v string)`

SetChallenge sets Challenge field to given value.

### HasChallenge

`func (o *CertificateVersion) HasChallenge() bool`

HasChallenge returns a boolean if a field has been set.

### GetAuthority

`func (o *CertificateVersion) GetAuthority() string`

GetAuthority returns the Authority field if non-nil, zero value otherwise.

### GetAuthorityOk

`func (o *CertificateVersion) GetAuthorityOk() (*string, bool)`

GetAuthorityOk returns a tuple with the Authority field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthority

`func (o *CertificateVersion) SetAuthority(v string)`

SetAuthority sets Authority field to given value.

### HasAuthority

`func (o *CertificateVersion) HasAuthority() bool`

HasAuthority returns a boolean if a field has been set.

### GetKeyAlgorithm

`func (o *CertificateVersion) GetKeyAlgorithm() string`

GetKeyAlgorithm returns the KeyAlgorithm field if non-nil, zero value otherwise.

### GetKeyAlgorithmOk

`func (o *CertificateVersion) GetKeyAlgorithmOk() (*string, bool)`

GetKeyAlgorithmOk returns a tuple with the KeyAlgorithm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKeyAlgorithm

`func (o *CertificateVersion) SetKeyAlgorithm(v string)`

SetKeyAlgorithm sets KeyAlgorithm field to given value.

### HasKeyAlgorithm

`func (o *CertificateVersion) HasKeyAlgorithm() bool`

HasKeyAlgorithm returns a boolean if a field has been set.

### GetLastEditor

`func (o *CertificateVersion) GetLastEditor() string`

GetLastEditor returns the LastEditor field if non-nil, zero value otherwise.

### GetLastEditorOk

`func (o *CertificateVersion) GetLastEditorOk() (*string, bool)`

GetLastEditorOk returns a tuple with the LastEditor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEditor

`func (o *CertificateVersion) SetLastEditor(v string)`

SetLastEditor sets LastEditor field to given value.

### HasLastEditor

`func (o *CertificateVersion) HasLastEditor() bool`

HasLastEditor returns a boolean if a field has been set.

### GetLastModified

`func (o *CertificateVersion) GetLastModified() time.Time`

GetLastModified returns the LastModified field if non-nil, zero value otherwise.

### GetLastModifiedOk

`func (o *CertificateVersion) GetLastModifiedOk() (*time.Time, bool)`

GetLastModifiedOk returns a tuple with the LastModified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastModified

`func (o *CertificateVersion) SetLastModified(v time.Time)`

SetLastModified sets LastModified field to given value.

### HasLastModified

`func (o *CertificateVersion) HasLastModified() bool`

HasLastModified returns a boolean if a field has been set.

### GetRenewedAt

`func (o *CertificateVersion) GetRenewedAt() time.Time`

GetRenewedAt returns the RenewedAt field if non-nil, zero value otherwise.

### GetRenewedAtOk

`func (o *CertificateVersion) GetRenewedAtOk() (*time.Time, bool)`

GetRenewedAtOk returns a tuple with the RenewedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRenewedAt

`func (o *CertificateVersion) SetRenewedAt(v time.Time)`

SetRenewedAt sets RenewedAt field to given value.

### HasRenewedAt

`func (o *CertificateVersion) HasRenewedAt() bool`

HasRenewedAt returns a boolean if a field has been set.

### SetRenewedAtNil

`func (o *CertificateVersion) SetRenewedAtNil(b bool)`

 SetRenewedAtNil sets the value for RenewedAt to be an explicit nil

### UnsetRenewedAt
`func (o *CertificateVersion) UnsetRenewedAt()`

UnsetRenewedAt ensures that no value is present for RenewedAt, not even an explicit nil
### GetVersionId

`func (o *CertificateVersion) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *CertificateVersion) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *CertificateVersion) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *CertificateVersion) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### GetVersionState

`func (o *CertificateVersion) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *CertificateVersion) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *CertificateVersion) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *CertificateVersion) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetProductVersion

`func (o *CertificateVersion) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *CertificateVersion) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *CertificateVersion) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.

### HasProductVersion

`func (o *CertificateVersion) HasProductVersion() bool`

HasProductVersion returns a boolean if a field has been set.

### GetSourceVersionId

`func (o *CertificateVersion) GetSourceVersionId() string`

GetSourceVersionId returns the SourceVersionId field if non-nil, zero value otherwise.

### GetSourceVersionIdOk

`func (o *CertificateVersion) GetSourceVersionIdOk() (*string, bool)`

GetSourceVersionIdOk returns a tuple with the SourceVersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceVersionId

`func (o *CertificateVersion) SetSourceVersionId(v string)`

SetSourceVersionId sets SourceVersionId field to given value.

### HasSourceVersionId

`func (o *CertificateVersion) HasSourceVersionId() bool`

HasSourceVersionId returns a boolean if a field has been set.

### SetSourceVersionIdNil

`func (o *CertificateVersion) SetSourceVersionIdNil(b bool)`

 SetSourceVersionIdNil sets the value for SourceVersionId to be an explicit nil

### UnsetSourceVersionId
`func (o *CertificateVersion) UnsetSourceVersionId()`

UnsetSourceVersionId ensures that no value is present for SourceVersionId, not even an explicit nil
### GetSnapshot

`func (o *CertificateVersion) GetSnapshot() map[string]interface{}`

GetSnapshot returns the Snapshot field if non-nil, zero value otherwise.

### GetSnapshotOk

`func (o *CertificateVersion) GetSnapshotOk() (*map[string]interface{}, bool)`

GetSnapshotOk returns a tuple with the Snapshot field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSnapshot

`func (o *CertificateVersion) SetSnapshot(v map[string]interface{})`

SetSnapshot sets Snapshot field to given value.

### HasSnapshot

`func (o *CertificateVersion) HasSnapshot() bool`

HasSnapshot returns a boolean if a field has been set.

### SetSnapshotNil

`func (o *CertificateVersion) SetSnapshotNil(b bool)`

 SetSnapshotNil sets the value for Snapshot to be an explicit nil

### UnsetSnapshot
`func (o *CertificateVersion) UnsetSnapshot()`

UnsetSnapshot ensures that no value is present for Snapshot, not even an explicit nil
### GetCreatedAt

`func (o *CertificateVersion) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *CertificateVersion) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *CertificateVersion) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *CertificateVersion) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetReadyAt

`func (o *CertificateVersion) GetReadyAt() time.Time`

GetReadyAt returns the ReadyAt field if non-nil, zero value otherwise.

### GetReadyAtOk

`func (o *CertificateVersion) GetReadyAtOk() (*time.Time, bool)`

GetReadyAtOk returns a tuple with the ReadyAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadyAt

`func (o *CertificateVersion) SetReadyAt(v time.Time)`

SetReadyAt sets ReadyAt field to given value.

### HasReadyAt

`func (o *CertificateVersion) HasReadyAt() bool`

HasReadyAt returns a boolean if a field has been set.

### SetReadyAtNil

`func (o *CertificateVersion) SetReadyAtNil(b bool)`

 SetReadyAtNil sets the value for ReadyAt to be an explicit nil

### UnsetReadyAt
`func (o *CertificateVersion) UnsetReadyAt()`

UnsetReadyAt ensures that no value is present for ReadyAt, not even an explicit nil
### GetDescription

`func (o *CertificateVersion) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CertificateVersion) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CertificateVersion) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CertificateVersion) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetBuildAt

`func (o *CertificateVersion) GetBuildAt() time.Time`

GetBuildAt returns the BuildAt field if non-nil, zero value otherwise.

### GetBuildAtOk

`func (o *CertificateVersion) GetBuildAtOk() (*time.Time, bool)`

GetBuildAtOk returns a tuple with the BuildAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildAt

`func (o *CertificateVersion) SetBuildAt(v time.Time)`

SetBuildAt sets BuildAt field to given value.

### HasBuildAt

`func (o *CertificateVersion) HasBuildAt() bool`

HasBuildAt returns a boolean if a field has been set.

### SetBuildAtNil

`func (o *CertificateVersion) SetBuildAtNil(b bool)`

 SetBuildAtNil sets the value for BuildAt to be an explicit nil

### UnsetBuildAt
`func (o *CertificateVersion) UnsetBuildAt()`

UnsetBuildAt ensures that no value is present for BuildAt, not even an explicit nil
### GetBuildComment

`func (o *CertificateVersion) GetBuildComment() string`

GetBuildComment returns the BuildComment field if non-nil, zero value otherwise.

### GetBuildCommentOk

`func (o *CertificateVersion) GetBuildCommentOk() (*string, bool)`

GetBuildCommentOk returns a tuple with the BuildComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildComment

`func (o *CertificateVersion) SetBuildComment(v string)`

SetBuildComment sets BuildComment field to given value.

### HasBuildComment

`func (o *CertificateVersion) HasBuildComment() bool`

HasBuildComment returns a boolean if a field has been set.

### GetCancelAt

`func (o *CertificateVersion) GetCancelAt() time.Time`

GetCancelAt returns the CancelAt field if non-nil, zero value otherwise.

### GetCancelAtOk

`func (o *CertificateVersion) GetCancelAtOk() (*time.Time, bool)`

GetCancelAtOk returns a tuple with the CancelAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelAt

`func (o *CertificateVersion) SetCancelAt(v time.Time)`

SetCancelAt sets CancelAt field to given value.

### HasCancelAt

`func (o *CertificateVersion) HasCancelAt() bool`

HasCancelAt returns a boolean if a field has been set.

### SetCancelAtNil

`func (o *CertificateVersion) SetCancelAtNil(b bool)`

 SetCancelAtNil sets the value for CancelAt to be an explicit nil

### UnsetCancelAt
`func (o *CertificateVersion) UnsetCancelAt()`

UnsetCancelAt ensures that no value is present for CancelAt, not even an explicit nil
### GetCancelComment

`func (o *CertificateVersion) GetCancelComment() string`

GetCancelComment returns the CancelComment field if non-nil, zero value otherwise.

### GetCancelCommentOk

`func (o *CertificateVersion) GetCancelCommentOk() (*string, bool)`

GetCancelCommentOk returns a tuple with the CancelComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelComment

`func (o *CertificateVersion) SetCancelComment(v string)`

SetCancelComment sets CancelComment field to given value.

### HasCancelComment

`func (o *CertificateVersion) HasCancelComment() bool`

HasCancelComment returns a boolean if a field has been set.

### GetArchivedAt

`func (o *CertificateVersion) GetArchivedAt() time.Time`

GetArchivedAt returns the ArchivedAt field if non-nil, zero value otherwise.

### GetArchivedAtOk

`func (o *CertificateVersion) GetArchivedAtOk() (*time.Time, bool)`

GetArchivedAtOk returns a tuple with the ArchivedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchivedAt

`func (o *CertificateVersion) SetArchivedAt(v time.Time)`

SetArchivedAt sets ArchivedAt field to given value.

### HasArchivedAt

`func (o *CertificateVersion) HasArchivedAt() bool`

HasArchivedAt returns a boolean if a field has been set.

### SetArchivedAtNil

`func (o *CertificateVersion) SetArchivedAtNil(b bool)`

 SetArchivedAtNil sets the value for ArchivedAt to be an explicit nil

### UnsetArchivedAt
`func (o *CertificateVersion) UnsetArchivedAt()`

UnsetArchivedAt ensures that no value is present for ArchivedAt, not even an explicit nil
### GetArchiveComment

`func (o *CertificateVersion) GetArchiveComment() string`

GetArchiveComment returns the ArchiveComment field if non-nil, zero value otherwise.

### GetArchiveCommentOk

`func (o *CertificateVersion) GetArchiveCommentOk() (*string, bool)`

GetArchiveCommentOk returns a tuple with the ArchiveComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchiveComment

`func (o *CertificateVersion) SetArchiveComment(v string)`

SetArchiveComment sets ArchiveComment field to given value.

### HasArchiveComment

`func (o *CertificateVersion) HasArchiveComment() bool`

HasArchiveComment returns a boolean if a field has been set.

### GetLastError

`func (o *CertificateVersion) GetLastError() map[string]interface{}`

GetLastError returns the LastError field if non-nil, zero value otherwise.

### GetLastErrorOk

`func (o *CertificateVersion) GetLastErrorOk() (*map[string]interface{}, bool)`

GetLastErrorOk returns a tuple with the LastError field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastError

`func (o *CertificateVersion) SetLastError(v map[string]interface{})`

SetLastError sets LastError field to given value.

### HasLastError

`func (o *CertificateVersion) HasLastError() bool`

HasLastError returns a boolean if a field has been set.

### SetLastErrorNil

`func (o *CertificateVersion) SetLastErrorNil(b bool)`

 SetLastErrorNil sets the value for LastError to be an explicit nil

### UnsetLastError
`func (o *CertificateVersion) UnsetLastError()`

UnsetLastError ensures that no value is present for LastError, not even an explicit nil
### GetTraceId

`func (o *CertificateVersion) GetTraceId() string`

GetTraceId returns the TraceId field if non-nil, zero value otherwise.

### GetTraceIdOk

`func (o *CertificateVersion) GetTraceIdOk() (*string, bool)`

GetTraceIdOk returns a tuple with the TraceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraceId

`func (o *CertificateVersion) SetTraceId(v string)`

SetTraceId sets TraceId field to given value.

### HasTraceId

`func (o *CertificateVersion) HasTraceId() bool`

HasTraceId returns a boolean if a field has been set.

### GetDependencies

`func (o *CertificateVersion) GetDependencies() []map[string][]ApplicationVersionDependenciesInnerValueInner`

GetDependencies returns the Dependencies field if non-nil, zero value otherwise.

### GetDependenciesOk

`func (o *CertificateVersion) GetDependenciesOk() (*[]map[string][]ApplicationVersionDependenciesInnerValueInner, bool)`

GetDependenciesOk returns a tuple with the Dependencies field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDependencies

`func (o *CertificateVersion) SetDependencies(v []map[string][]ApplicationVersionDependenciesInnerValueInner)`

SetDependencies sets Dependencies field to given value.

### HasDependencies

`func (o *CertificateVersion) HasDependencies() bool`

HasDependencies returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


