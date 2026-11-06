# FirewallVersionCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Modules** | Pointer to [**FirewallModulesRequest**](FirewallModulesRequest.md) |  | [optional] 
**Debug** | Pointer to **bool** |  | [optional] 
**SourceVersion** | Pointer to **NullableString** | ID of the version to clone from. If omitted, clones latest ready. | [optional] 
**Comment** | Pointer to **string** | Accepted and not stored. | [optional] 

## Methods

### NewFirewallVersionCreateRequest

`func NewFirewallVersionCreateRequest() *FirewallVersionCreateRequest`

NewFirewallVersionCreateRequest instantiates a new FirewallVersionCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFirewallVersionCreateRequestWithDefaults

`func NewFirewallVersionCreateRequestWithDefaults() *FirewallVersionCreateRequest`

NewFirewallVersionCreateRequestWithDefaults instantiates a new FirewallVersionCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *FirewallVersionCreateRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *FirewallVersionCreateRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *FirewallVersionCreateRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *FirewallVersionCreateRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetModules

`func (o *FirewallVersionCreateRequest) GetModules() FirewallModulesRequest`

GetModules returns the Modules field if non-nil, zero value otherwise.

### GetModulesOk

`func (o *FirewallVersionCreateRequest) GetModulesOk() (*FirewallModulesRequest, bool)`

GetModulesOk returns a tuple with the Modules field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModules

`func (o *FirewallVersionCreateRequest) SetModules(v FirewallModulesRequest)`

SetModules sets Modules field to given value.

### HasModules

`func (o *FirewallVersionCreateRequest) HasModules() bool`

HasModules returns a boolean if a field has been set.

### GetDebug

`func (o *FirewallVersionCreateRequest) GetDebug() bool`

GetDebug returns the Debug field if non-nil, zero value otherwise.

### GetDebugOk

`func (o *FirewallVersionCreateRequest) GetDebugOk() (*bool, bool)`

GetDebugOk returns a tuple with the Debug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDebug

`func (o *FirewallVersionCreateRequest) SetDebug(v bool)`

SetDebug sets Debug field to given value.

### HasDebug

`func (o *FirewallVersionCreateRequest) HasDebug() bool`

HasDebug returns a boolean if a field has been set.

### GetSourceVersion

`func (o *FirewallVersionCreateRequest) GetSourceVersion() string`

GetSourceVersion returns the SourceVersion field if non-nil, zero value otherwise.

### GetSourceVersionOk

`func (o *FirewallVersionCreateRequest) GetSourceVersionOk() (*string, bool)`

GetSourceVersionOk returns a tuple with the SourceVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceVersion

`func (o *FirewallVersionCreateRequest) SetSourceVersion(v string)`

SetSourceVersion sets SourceVersion field to given value.

### HasSourceVersion

`func (o *FirewallVersionCreateRequest) HasSourceVersion() bool`

HasSourceVersion returns a boolean if a field has been set.

### SetSourceVersionNil

`func (o *FirewallVersionCreateRequest) SetSourceVersionNil(b bool)`

 SetSourceVersionNil sets the value for SourceVersion to be an explicit nil

### UnsetSourceVersion
`func (o *FirewallVersionCreateRequest) UnsetSourceVersion()`

UnsetSourceVersion ensures that no value is present for SourceVersion, not even an explicit nil
### GetComment

`func (o *FirewallVersionCreateRequest) GetComment() string`

GetComment returns the Comment field if non-nil, zero value otherwise.

### GetCommentOk

`func (o *FirewallVersionCreateRequest) GetCommentOk() (*string, bool)`

GetCommentOk returns a tuple with the Comment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetComment

`func (o *FirewallVersionCreateRequest) SetComment(v string)`

SetComment sets Comment field to given value.

### HasComment

`func (o *FirewallVersionCreateRequest) HasComment() bool`

HasComment returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


