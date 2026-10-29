# VariableVersionListItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**VersionId** | Pointer to **string** |  | [optional] 
**VariableId** | Pointer to **string** |  | [optional] 
**Action** | Pointer to **string** |  | [optional] 
**Key** | Pointer to **string** |  | [optional] 
**LastEditor** | Pointer to **string** |  | [optional] 
**CreatedAt** | **time.Time** |  | 
**SourceVersionId** | Pointer to **NullableString** |  | [optional] 
**BuildResourceVersion** | Pointer to **NullableString** |  | [optional] 
**BuildStatus** | Pointer to **NullableString** |  | [optional] 
**VersionState** | Pointer to **string** |  | [optional] 
**TraceId** | Pointer to **string** |  | [optional] 

## Methods

### NewVariableVersionListItem

`func NewVariableVersionListItem(createdAt time.Time, ) *VariableVersionListItem`

NewVariableVersionListItem instantiates a new VariableVersionListItem object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewVariableVersionListItemWithDefaults

`func NewVariableVersionListItemWithDefaults() *VariableVersionListItem`

NewVariableVersionListItemWithDefaults instantiates a new VariableVersionListItem object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersionId

`func (o *VariableVersionListItem) GetVersionId() string`

GetVersionId returns the VersionId field if non-nil, zero value otherwise.

### GetVersionIdOk

`func (o *VariableVersionListItem) GetVersionIdOk() (*string, bool)`

GetVersionIdOk returns a tuple with the VersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionId

`func (o *VariableVersionListItem) SetVersionId(v string)`

SetVersionId sets VersionId field to given value.

### HasVersionId

`func (o *VariableVersionListItem) HasVersionId() bool`

HasVersionId returns a boolean if a field has been set.

### GetVariableId

`func (o *VariableVersionListItem) GetVariableId() string`

GetVariableId returns the VariableId field if non-nil, zero value otherwise.

### GetVariableIdOk

`func (o *VariableVersionListItem) GetVariableIdOk() (*string, bool)`

GetVariableIdOk returns a tuple with the VariableId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVariableId

`func (o *VariableVersionListItem) SetVariableId(v string)`

SetVariableId sets VariableId field to given value.

### HasVariableId

`func (o *VariableVersionListItem) HasVariableId() bool`

HasVariableId returns a boolean if a field has been set.

### GetAction

`func (o *VariableVersionListItem) GetAction() string`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *VariableVersionListItem) GetActionOk() (*string, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *VariableVersionListItem) SetAction(v string)`

SetAction sets Action field to given value.

### HasAction

`func (o *VariableVersionListItem) HasAction() bool`

HasAction returns a boolean if a field has been set.

### GetKey

`func (o *VariableVersionListItem) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *VariableVersionListItem) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *VariableVersionListItem) SetKey(v string)`

SetKey sets Key field to given value.

### HasKey

`func (o *VariableVersionListItem) HasKey() bool`

HasKey returns a boolean if a field has been set.

### GetLastEditor

`func (o *VariableVersionListItem) GetLastEditor() string`

GetLastEditor returns the LastEditor field if non-nil, zero value otherwise.

### GetLastEditorOk

`func (o *VariableVersionListItem) GetLastEditorOk() (*string, bool)`

GetLastEditorOk returns a tuple with the LastEditor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEditor

`func (o *VariableVersionListItem) SetLastEditor(v string)`

SetLastEditor sets LastEditor field to given value.

### HasLastEditor

`func (o *VariableVersionListItem) HasLastEditor() bool`

HasLastEditor returns a boolean if a field has been set.

### GetCreatedAt

`func (o *VariableVersionListItem) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *VariableVersionListItem) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *VariableVersionListItem) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetSourceVersionId

`func (o *VariableVersionListItem) GetSourceVersionId() string`

GetSourceVersionId returns the SourceVersionId field if non-nil, zero value otherwise.

### GetSourceVersionIdOk

`func (o *VariableVersionListItem) GetSourceVersionIdOk() (*string, bool)`

GetSourceVersionIdOk returns a tuple with the SourceVersionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceVersionId

`func (o *VariableVersionListItem) SetSourceVersionId(v string)`

SetSourceVersionId sets SourceVersionId field to given value.

### HasSourceVersionId

`func (o *VariableVersionListItem) HasSourceVersionId() bool`

HasSourceVersionId returns a boolean if a field has been set.

### SetSourceVersionIdNil

`func (o *VariableVersionListItem) SetSourceVersionIdNil(b bool)`

 SetSourceVersionIdNil sets the value for SourceVersionId to be an explicit nil

### UnsetSourceVersionId
`func (o *VariableVersionListItem) UnsetSourceVersionId()`

UnsetSourceVersionId ensures that no value is present for SourceVersionId, not even an explicit nil
### GetBuildResourceVersion

`func (o *VariableVersionListItem) GetBuildResourceVersion() string`

GetBuildResourceVersion returns the BuildResourceVersion field if non-nil, zero value otherwise.

### GetBuildResourceVersionOk

`func (o *VariableVersionListItem) GetBuildResourceVersionOk() (*string, bool)`

GetBuildResourceVersionOk returns a tuple with the BuildResourceVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildResourceVersion

`func (o *VariableVersionListItem) SetBuildResourceVersion(v string)`

SetBuildResourceVersion sets BuildResourceVersion field to given value.

### HasBuildResourceVersion

`func (o *VariableVersionListItem) HasBuildResourceVersion() bool`

HasBuildResourceVersion returns a boolean if a field has been set.

### SetBuildResourceVersionNil

`func (o *VariableVersionListItem) SetBuildResourceVersionNil(b bool)`

 SetBuildResourceVersionNil sets the value for BuildResourceVersion to be an explicit nil

### UnsetBuildResourceVersion
`func (o *VariableVersionListItem) UnsetBuildResourceVersion()`

UnsetBuildResourceVersion ensures that no value is present for BuildResourceVersion, not even an explicit nil
### GetBuildStatus

`func (o *VariableVersionListItem) GetBuildStatus() string`

GetBuildStatus returns the BuildStatus field if non-nil, zero value otherwise.

### GetBuildStatusOk

`func (o *VariableVersionListItem) GetBuildStatusOk() (*string, bool)`

GetBuildStatusOk returns a tuple with the BuildStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBuildStatus

`func (o *VariableVersionListItem) SetBuildStatus(v string)`

SetBuildStatus sets BuildStatus field to given value.

### HasBuildStatus

`func (o *VariableVersionListItem) HasBuildStatus() bool`

HasBuildStatus returns a boolean if a field has been set.

### SetBuildStatusNil

`func (o *VariableVersionListItem) SetBuildStatusNil(b bool)`

 SetBuildStatusNil sets the value for BuildStatus to be an explicit nil

### UnsetBuildStatus
`func (o *VariableVersionListItem) UnsetBuildStatus()`

UnsetBuildStatus ensures that no value is present for BuildStatus, not even an explicit nil
### GetVersionState

`func (o *VariableVersionListItem) GetVersionState() string`

GetVersionState returns the VersionState field if non-nil, zero value otherwise.

### GetVersionStateOk

`func (o *VariableVersionListItem) GetVersionStateOk() (*string, bool)`

GetVersionStateOk returns a tuple with the VersionState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersionState

`func (o *VariableVersionListItem) SetVersionState(v string)`

SetVersionState sets VersionState field to given value.

### HasVersionState

`func (o *VariableVersionListItem) HasVersionState() bool`

HasVersionState returns a boolean if a field has been set.

### GetTraceId

`func (o *VariableVersionListItem) GetTraceId() string`

GetTraceId returns the TraceId field if non-nil, zero value otherwise.

### GetTraceIdOk

`func (o *VariableVersionListItem) GetTraceIdOk() (*string, bool)`

GetTraceIdOk returns a tuple with the TraceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraceId

`func (o *VariableVersionListItem) SetTraceId(v string)`

SetTraceId sets TraceId field to given value.

### HasTraceId

`func (o *VariableVersionListItem) HasTraceId() bool`

HasTraceId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


