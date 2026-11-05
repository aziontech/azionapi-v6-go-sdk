# CertificateRevocationListVersionList

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**VersionId** | Pointer to **string** | ID of the version metadata. | [optional] 
**VersionState** | Pointer to **string** | Current lifecycle state of the version. | [optional] 
**CreatedAt** | Pointer to **NullableTime** | When this version was created | [optional] 
**ReadyAt** | Pointer to **NullableTime** | When this version became ready | [optional] 
**Description** | Pointer to **string** | Version description | [optional] 
**LastEditor** | Pointer to **NullableString** | Email of the last editor | [optional] 

## Methods

### NewCertificateRevocationListVersionList

`func NewCertificateRevocationListVersionList() *CertificateRevocationListVersionList`

NewCertificateRevocationListVersionList instantiates a new CertificateRevocationListVersionList object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCertificateRevocationListVersionListWithDefaults

`func NewCertificateRevocationListVersionListWithDefaults() *CertificateRevocationListVersionList`

NewCertificateRevocationListVersionListWithDefaults instantiates a new CertificateRevocationListVersionList object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersionId

`func (o *CertificateRevocationListVersionList) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *CertificateRevocationListVersionList) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *CertificateRevocationListVersionList) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *CertificateRevocationListVersionList) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### GetVersionState

`func (o *CertificateRevocationListVersionList) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *CertificateRevocationListVersionList) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *CertificateRevocationListVersionList) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *CertificateRevocationListVersionList) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetCreatedAt

`func (o *CertificateRevocationListVersionList) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *CertificateRevocationListVersionList) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *CertificateRevocationListVersionList) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *CertificateRevocationListVersionList) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### SetCreatedAtNil

`func (o *CertificateRevocationListVersionList) SetCreatedAtNil(b bool)`

 SetCreatedAtNil sets the value for CreatedAt to be an explicit nil

### UnsetCreatedAt
`func (o *CertificateRevocationListVersionList) UnsetCreatedAt()`

UnsetCreatedAt ensures that no value is present for CreatedAt, not even an explicit nil
### GetReadyAt

`func (o *CertificateRevocationListVersionList) GetReadyAt() time.Time`

GetReadyAt returns the ReadyAt field if non-nil, zero value otherwise.

### GetReadyAtOk

`func (o *CertificateRevocationListVersionList) GetReadyAtOk() (*time.Time, bool)`

GetReadyAtOk returns a tuple with the ReadyAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadyAt

`func (o *CertificateRevocationListVersionList) SetReadyAt(v time.Time)`

SetReadyAt sets ReadyAt field to given value.

### HasReadyAt

`func (o *CertificateRevocationListVersionList) HasReadyAt() bool`

HasReadyAt returns a boolean if a field has been set.

### SetReadyAtNil

`func (o *CertificateRevocationListVersionList) SetReadyAtNil(b bool)`

 SetReadyAtNil sets the value for ReadyAt to be an explicit nil

### UnsetReadyAt
`func (o *CertificateRevocationListVersionList) UnsetReadyAt()`

UnsetReadyAt ensures that no value is present for ReadyAt, not even an explicit nil
### GetDescription

`func (o *CertificateRevocationListVersionList) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CertificateRevocationListVersionList) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CertificateRevocationListVersionList) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CertificateRevocationListVersionList) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetLastEditor

`func (o *CertificateRevocationListVersionList) GetLastEditor() string`

GetLastEditor returns the LastEditor field if non-nil, zero value otherwise.

### GetLastEditorOk

`func (o *CertificateRevocationListVersionList) GetLastEditorOk() (*string, bool)`

GetLastEditorOk returns a tuple with the LastEditor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEditor

`func (o *CertificateRevocationListVersionList) SetLastEditor(v string)`

SetLastEditor sets LastEditor field to given value.

### HasLastEditor

`func (o *CertificateRevocationListVersionList) HasLastEditor() bool`

HasLastEditor returns a boolean if a field has been set.

### SetLastEditorNil

`func (o *CertificateRevocationListVersionList) SetLastEditorNil(b bool)`

 SetLastEditorNil sets the value for LastEditor to be an explicit nil

### UnsetLastEditor
`func (o *CertificateRevocationListVersionList) UnsetLastEditor()`

UnsetLastEditor ensures that no value is present for LastEditor, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


