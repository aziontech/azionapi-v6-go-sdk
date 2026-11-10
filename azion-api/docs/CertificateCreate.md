# CertificateCreate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **int64** |  | [optional] 
**Name** | **string** |  | 
**Certificate** | **string** |  | 
**PrivateKey** | Pointer to **NullableString** | Required for a certificate, not for a trusted_ca_certificate. | [optional] 
**Issuer** | Pointer to **NullableString** |  | [optional] 
**SubjectName** | Pointer to **[]string** |  | [optional] 
**Validity** | Pointer to **NullableString** |  | [optional] 
**Type** | Pointer to **string** | The value can&#39;t be changed after the certificate creation.  * &#x60;edge_certificate&#x60; - Certificate * &#x60;trusted_ca_certificate&#x60; - Trusted CA Certificate | [optional] 
**Managed** | Pointer to **bool** |  | [optional] 
**Csr** | Pointer to **NullableString** |  | [optional] 
**Challenge** | Pointer to **string** |  | [optional] 
**Authority** | Pointer to **string** |  | [optional] 
**KeyAlgorithm** | Pointer to **string** |  | [optional] 
**ProductVersion** | Pointer to **string** |  | [optional] 
**LastEditor** | Pointer to **string** |  | [optional] 
**CreatedAt** | Pointer to **NullableTime** | Timestamp of the certificate creation on the platform. | [optional] 
**LastModified** | Pointer to **time.Time** | Timestamp of the last modification made to the certificate content on the platform. | [optional] 
**RenewedAt** | Pointer to **NullableTime** | Timestamp indicating when the managed certificate was renewed on our platform. | [optional] 
**VersionId** | Pointer to **NullableString** | ID of the version metadata (use in /versions/{id} URLs) | [optional] 
**VersionState** | Pointer to **NullableString** | Build state of this version (queued, building, ready, error, ...) | [optional] 

## Methods

### NewCertificateCreate

`func NewCertificateCreate(name string, certificate string, ) *CertificateCreate`

NewCertificateCreate instantiates a new CertificateCreate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCertificateCreateWithDefaults

`func NewCertificateCreateWithDefaults() *CertificateCreate`

NewCertificateCreateWithDefaults instantiates a new CertificateCreate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *CertificateCreate) GetId() int64`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *CertificateCreate) GetIdOk() (*int64, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *CertificateCreate) SetId(v int64)`

SetId sets Id field to given value.

### HasId

`func (o *CertificateCreate) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *CertificateCreate) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CertificateCreate) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CertificateCreate) SetName(v string)`

SetName sets Name field to given value.


### GetCertificate

`func (o *CertificateCreate) GetCertificate() string`

GetCertificate returns the Certificate field if non-nil, zero value otherwise.

### GetCertificateOk

`func (o *CertificateCreate) GetCertificateOk() (*string, bool)`

GetCertificateOk returns a tuple with the Certificate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCertificate

`func (o *CertificateCreate) SetCertificate(v string)`

SetCertificate sets Certificate field to given value.


### GetPrivateKey

`func (o *CertificateCreate) GetPrivateKey() string`

GetPrivateKey returns the PrivateKey field if non-nil, zero value otherwise.

### GetPrivateKeyOk

`func (o *CertificateCreate) GetPrivateKeyOk() (*string, bool)`

GetPrivateKeyOk returns a tuple with the PrivateKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrivateKey

`func (o *CertificateCreate) SetPrivateKey(v string)`

SetPrivateKey sets PrivateKey field to given value.

### HasPrivateKey

`func (o *CertificateCreate) HasPrivateKey() bool`

HasPrivateKey returns a boolean if a field has been set.

### SetPrivateKeyNil

`func (o *CertificateCreate) SetPrivateKeyNil(b bool)`

 SetPrivateKeyNil sets the value for PrivateKey to be an explicit nil

### UnsetPrivateKey
`func (o *CertificateCreate) UnsetPrivateKey()`

UnsetPrivateKey ensures that no value is present for PrivateKey, not even an explicit nil
### GetIssuer

`func (o *CertificateCreate) GetIssuer() string`

GetIssuer returns the Issuer field if non-nil, zero value otherwise.

### GetIssuerOk

`func (o *CertificateCreate) GetIssuerOk() (*string, bool)`

GetIssuerOk returns a tuple with the Issuer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssuer

`func (o *CertificateCreate) SetIssuer(v string)`

SetIssuer sets Issuer field to given value.

### HasIssuer

`func (o *CertificateCreate) HasIssuer() bool`

HasIssuer returns a boolean if a field has been set.

### SetIssuerNil

`func (o *CertificateCreate) SetIssuerNil(b bool)`

 SetIssuerNil sets the value for Issuer to be an explicit nil

### UnsetIssuer
`func (o *CertificateCreate) UnsetIssuer()`

UnsetIssuer ensures that no value is present for Issuer, not even an explicit nil
### GetSubjectName

`func (o *CertificateCreate) GetSubjectName() []string`

GetSubjectName returns the SubjectName field if non-nil, zero value otherwise.

### GetSubjectNameOk

`func (o *CertificateCreate) GetSubjectNameOk() (*[]string, bool)`

GetSubjectNameOk returns a tuple with the SubjectName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubjectName

`func (o *CertificateCreate) SetSubjectName(v []string)`

SetSubjectName sets SubjectName field to given value.

### HasSubjectName

`func (o *CertificateCreate) HasSubjectName() bool`

HasSubjectName returns a boolean if a field has been set.

### GetValidity

`func (o *CertificateCreate) GetValidity() string`

GetValidity returns the Validity field if non-nil, zero value otherwise.

### GetValidityOk

`func (o *CertificateCreate) GetValidityOk() (*string, bool)`

GetValidityOk returns a tuple with the Validity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValidity

`func (o *CertificateCreate) SetValidity(v string)`

SetValidity sets Validity field to given value.

### HasValidity

`func (o *CertificateCreate) HasValidity() bool`

HasValidity returns a boolean if a field has been set.

### SetValidityNil

`func (o *CertificateCreate) SetValidityNil(b bool)`

 SetValidityNil sets the value for Validity to be an explicit nil

### UnsetValidity
`func (o *CertificateCreate) UnsetValidity()`

UnsetValidity ensures that no value is present for Validity, not even an explicit nil
### GetType

`func (o *CertificateCreate) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CertificateCreate) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CertificateCreate) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *CertificateCreate) HasType() bool`

HasType returns a boolean if a field has been set.

### GetManaged

`func (o *CertificateCreate) GetManaged() bool`

GetManaged returns the Managed field if non-nil, zero value otherwise.

### GetManagedOk

`func (o *CertificateCreate) GetManagedOk() (*bool, bool)`

GetManagedOk returns a tuple with the Managed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetManaged

`func (o *CertificateCreate) SetManaged(v bool)`

SetManaged sets Managed field to given value.

### HasManaged

`func (o *CertificateCreate) HasManaged() bool`

HasManaged returns a boolean if a field has been set.

### GetCsr

`func (o *CertificateCreate) GetCsr() string`

GetCsr returns the Csr field if non-nil, zero value otherwise.

### GetCsrOk

`func (o *CertificateCreate) GetCsrOk() (*string, bool)`

GetCsrOk returns a tuple with the Csr field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCsr

`func (o *CertificateCreate) SetCsr(v string)`

SetCsr sets Csr field to given value.

### HasCsr

`func (o *CertificateCreate) HasCsr() bool`

HasCsr returns a boolean if a field has been set.

### SetCsrNil

`func (o *CertificateCreate) SetCsrNil(b bool)`

 SetCsrNil sets the value for Csr to be an explicit nil

### UnsetCsr
`func (o *CertificateCreate) UnsetCsr()`

UnsetCsr ensures that no value is present for Csr, not even an explicit nil
### GetChallenge

`func (o *CertificateCreate) GetChallenge() string`

GetChallenge returns the Challenge field if non-nil, zero value otherwise.

### GetChallengeOk

`func (o *CertificateCreate) GetChallengeOk() (*string, bool)`

GetChallengeOk returns a tuple with the Challenge field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChallenge

`func (o *CertificateCreate) SetChallenge(v string)`

SetChallenge sets Challenge field to given value.

### HasChallenge

`func (o *CertificateCreate) HasChallenge() bool`

HasChallenge returns a boolean if a field has been set.

### GetAuthority

`func (o *CertificateCreate) GetAuthority() string`

GetAuthority returns the Authority field if non-nil, zero value otherwise.

### GetAuthorityOk

`func (o *CertificateCreate) GetAuthorityOk() (*string, bool)`

GetAuthorityOk returns a tuple with the Authority field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthority

`func (o *CertificateCreate) SetAuthority(v string)`

SetAuthority sets Authority field to given value.

### HasAuthority

`func (o *CertificateCreate) HasAuthority() bool`

HasAuthority returns a boolean if a field has been set.

### GetKeyAlgorithm

`func (o *CertificateCreate) GetKeyAlgorithm() string`

GetKeyAlgorithm returns the KeyAlgorithm field if non-nil, zero value otherwise.

### GetKeyAlgorithmOk

`func (o *CertificateCreate) GetKeyAlgorithmOk() (*string, bool)`

GetKeyAlgorithmOk returns a tuple with the KeyAlgorithm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKeyAlgorithm

`func (o *CertificateCreate) SetKeyAlgorithm(v string)`

SetKeyAlgorithm sets KeyAlgorithm field to given value.

### HasKeyAlgorithm

`func (o *CertificateCreate) HasKeyAlgorithm() bool`

HasKeyAlgorithm returns a boolean if a field has been set.

### GetProductVersion

`func (o *CertificateCreate) GetProductVersion() string`

GetProductVersion returns the ProductVersion field if non-nil, zero value otherwise.

### GetProductVersionOk

`func (o *CertificateCreate) GetProductVersionOk() (*string, bool)`

GetProductVersionOk returns a tuple with the ProductVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductVersion

`func (o *CertificateCreate) SetProductVersion(v string)`

SetProductVersion sets ProductVersion field to given value.

### HasProductVersion

`func (o *CertificateCreate) HasProductVersion() bool`

HasProductVersion returns a boolean if a field has been set.

### GetLastEditor

`func (o *CertificateCreate) GetLastEditor() string`

GetLastEditor returns the LastEditor field if non-nil, zero value otherwise.

### GetLastEditorOk

`func (o *CertificateCreate) GetLastEditorOk() (*string, bool)`

GetLastEditorOk returns a tuple with the LastEditor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEditor

`func (o *CertificateCreate) SetLastEditor(v string)`

SetLastEditor sets LastEditor field to given value.

### HasLastEditor

`func (o *CertificateCreate) HasLastEditor() bool`

HasLastEditor returns a boolean if a field has been set.

### GetCreatedAt

`func (o *CertificateCreate) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *CertificateCreate) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *CertificateCreate) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *CertificateCreate) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### SetCreatedAtNil

`func (o *CertificateCreate) SetCreatedAtNil(b bool)`

 SetCreatedAtNil sets the value for CreatedAt to be an explicit nil

### UnsetCreatedAt
`func (o *CertificateCreate) UnsetCreatedAt()`

UnsetCreatedAt ensures that no value is present for CreatedAt, not even an explicit nil
### GetLastModified

`func (o *CertificateCreate) GetLastModified() time.Time`

GetLastModified returns the LastModified field if non-nil, zero value otherwise.

### GetLastModifiedOk

`func (o *CertificateCreate) GetLastModifiedOk() (*time.Time, bool)`

GetLastModifiedOk returns a tuple with the LastModified field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastModified

`func (o *CertificateCreate) SetLastModified(v time.Time)`

SetLastModified sets LastModified field to given value.

### HasLastModified

`func (o *CertificateCreate) HasLastModified() bool`

HasLastModified returns a boolean if a field has been set.

### GetRenewedAt

`func (o *CertificateCreate) GetRenewedAt() time.Time`

GetRenewedAt returns the RenewedAt field if non-nil, zero value otherwise.

### GetRenewedAtOk

`func (o *CertificateCreate) GetRenewedAtOk() (*time.Time, bool)`

GetRenewedAtOk returns a tuple with the RenewedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRenewedAt

`func (o *CertificateCreate) SetRenewedAt(v time.Time)`

SetRenewedAt sets RenewedAt field to given value.

### HasRenewedAt

`func (o *CertificateCreate) HasRenewedAt() bool`

HasRenewedAt returns a boolean if a field has been set.

### SetRenewedAtNil

`func (o *CertificateCreate) SetRenewedAtNil(b bool)`

 SetRenewedAtNil sets the value for RenewedAt to be an explicit nil

### UnsetRenewedAt
`func (o *CertificateCreate) UnsetRenewedAt()`

UnsetRenewedAt ensures that no value is present for RenewedAt, not even an explicit nil
### GetVersionId

`func (o *CertificateCreate) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *CertificateCreate) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *CertificateCreate) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *CertificateCreate) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### SetVersionIdNil

`func (o *CertificateCreate) SetVersionIdNil(b bool)`

 SetVersionIdNil sets the value for VersionId to be an explicit nil

### UnsetVersionId
`func (o *CertificateCreate) UnsetVersionId()`

UnsetVersionId ensures that no value is present for VersionId, not even an explicit nil
### GetVersionState

`func (o *CertificateCreate) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *CertificateCreate) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *CertificateCreate) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *CertificateCreate) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### SetVersionStateNil

`func (o *CertificateCreate) SetVersionStateNil(b bool)`

 SetVersionStateNil sets the value for VersionState to be an explicit nil

### UnsetVersionState
`func (o *CertificateCreate) UnsetVersionState()`

UnsetVersionState ensures that no value is present for VersionState, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


