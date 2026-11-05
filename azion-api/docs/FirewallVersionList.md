# FirewallVersionList

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

### NewFirewallVersionList

`func NewFirewallVersionList() *FirewallVersionList`

NewFirewallVersionList instantiates a new FirewallVersionList object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFirewallVersionListWithDefaults

`func NewFirewallVersionListWithDefaults() *FirewallVersionList`

NewFirewallVersionListWithDefaults instantiates a new FirewallVersionList object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersionId

`func (o *FirewallVersionList) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *FirewallVersionList) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *FirewallVersionList) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *FirewallVersionList) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### GetVersionState

`func (o *FirewallVersionList) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *FirewallVersionList) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *FirewallVersionList) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *FirewallVersionList) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetCreatedAt

`func (o *FirewallVersionList) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *FirewallVersionList) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *FirewallVersionList) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *FirewallVersionList) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### SetCreatedAtNil

`func (o *FirewallVersionList) SetCreatedAtNil(b bool)`

 SetCreatedAtNil sets the value for CreatedAt to be an explicit nil

### UnsetCreatedAt
`func (o *FirewallVersionList) UnsetCreatedAt()`

UnsetCreatedAt ensures that no value is present for CreatedAt, not even an explicit nil
### GetReadyAt

`func (o *FirewallVersionList) GetReadyAt() time.Time`

GetReadyAt returns the ReadyAt field if non-nil, zero value otherwise.

### GetReadyAtOk

`func (o *FirewallVersionList) GetReadyAtOk() (*time.Time, bool)`

GetReadyAtOk returns a tuple with the ReadyAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadyAt

`func (o *FirewallVersionList) SetReadyAt(v time.Time)`

SetReadyAt sets ReadyAt field to given value.

### HasReadyAt

`func (o *FirewallVersionList) HasReadyAt() bool`

HasReadyAt returns a boolean if a field has been set.

### SetReadyAtNil

`func (o *FirewallVersionList) SetReadyAtNil(b bool)`

 SetReadyAtNil sets the value for ReadyAt to be an explicit nil

### UnsetReadyAt
`func (o *FirewallVersionList) UnsetReadyAt()`

UnsetReadyAt ensures that no value is present for ReadyAt, not even an explicit nil
### GetDescription

`func (o *FirewallVersionList) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *FirewallVersionList) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *FirewallVersionList) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *FirewallVersionList) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetLastEditor

`func (o *FirewallVersionList) GetLastEditor() string`

GetLastEditor returns the LastEditor field if non-nil, zero value otherwise.

### GetLastEditorOk

`func (o *FirewallVersionList) GetLastEditorOk() (*string, bool)`

GetLastEditorOk returns a tuple with the LastEditor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEditor

`func (o *FirewallVersionList) SetLastEditor(v string)`

SetLastEditor sets LastEditor field to given value.

### HasLastEditor

`func (o *FirewallVersionList) HasLastEditor() bool`

HasLastEditor returns a boolean if a field has been set.

### SetLastEditorNil

`func (o *FirewallVersionList) SetLastEditorNil(b bool)`

 SetLastEditorNil sets the value for LastEditor to be an explicit nil

### UnsetLastEditor
`func (o *FirewallVersionList) UnsetLastEditor()`

UnsetLastEditor ensures that no value is present for LastEditor, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


