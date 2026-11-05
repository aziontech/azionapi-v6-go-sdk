# ApplicationVersionCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Modules** | Pointer to [**ApplicationModulesRequest**](ApplicationModulesRequest.md) |  | [optional] 
**Active** | Pointer to **bool** |  | [optional] 
**Debug** | Pointer to **bool** |  | [optional] 
**SourceVersion** | Pointer to **NullableString** | ID of the version to clone from. If omitted, clones latest ready. | [optional] 
**Comment** | Pointer to **string** | Accepted and not stored. | [optional] 

## Methods

### NewApplicationVersionCreateRequest

`func NewApplicationVersionCreateRequest() *ApplicationVersionCreateRequest`

NewApplicationVersionCreateRequest instantiates a new ApplicationVersionCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApplicationVersionCreateRequestWithDefaults

`func NewApplicationVersionCreateRequestWithDefaults() *ApplicationVersionCreateRequest`

NewApplicationVersionCreateRequestWithDefaults instantiates a new ApplicationVersionCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *ApplicationVersionCreateRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ApplicationVersionCreateRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ApplicationVersionCreateRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ApplicationVersionCreateRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetModules

`func (o *ApplicationVersionCreateRequest) GetModules() ApplicationModulesRequest`

GetModules returns the Modules field if non-nil, zero value otherwise.

### GetModulesOk

`func (o *ApplicationVersionCreateRequest) GetModulesOk() (*ApplicationModulesRequest, bool)`

GetModulesOk returns a tuple with the Modules field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModules

`func (o *ApplicationVersionCreateRequest) SetModules(v ApplicationModulesRequest)`

SetModules sets Modules field to given value.

### HasModules

`func (o *ApplicationVersionCreateRequest) HasModules() bool`

HasModules returns a boolean if a field has been set.

### GetActive

`func (o *ApplicationVersionCreateRequest) GetActive() bool`

GetActive returns the Active field if non-nil, zero value otherwise.

### GetActiveOk

`func (o *ApplicationVersionCreateRequest) GetActiveOk() (*bool, bool)`

GetActiveOk returns a tuple with the Active field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActive

`func (o *ApplicationVersionCreateRequest) SetActive(v bool)`

SetActive sets Active field to given value.

### HasActive

`func (o *ApplicationVersionCreateRequest) HasActive() bool`

HasActive returns a boolean if a field has been set.

### GetDebug

`func (o *ApplicationVersionCreateRequest) GetDebug() bool`

GetDebug returns the Debug field if non-nil, zero value otherwise.

### GetDebugOk

`func (o *ApplicationVersionCreateRequest) GetDebugOk() (*bool, bool)`

GetDebugOk returns a tuple with the Debug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDebug

`func (o *ApplicationVersionCreateRequest) SetDebug(v bool)`

SetDebug sets Debug field to given value.

### HasDebug

`func (o *ApplicationVersionCreateRequest) HasDebug() bool`

HasDebug returns a boolean if a field has been set.

### GetSourceVersion

`func (o *ApplicationVersionCreateRequest) GetSourceVersion() string`

GetSourceVersion returns the SourceVersion field if non-nil, zero value otherwise.

### GetSourceVersionOk

`func (o *ApplicationVersionCreateRequest) GetSourceVersionOk() (*string, bool)`

GetSourceVersionOk returns a tuple with the SourceVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceVersion

`func (o *ApplicationVersionCreateRequest) SetSourceVersion(v string)`

SetSourceVersion sets SourceVersion field to given value.

### HasSourceVersion

`func (o *ApplicationVersionCreateRequest) HasSourceVersion() bool`

HasSourceVersion returns a boolean if a field has been set.

### SetSourceVersionNil

`func (o *ApplicationVersionCreateRequest) SetSourceVersionNil(b bool)`

 SetSourceVersionNil sets the value for SourceVersion to be an explicit nil

### UnsetSourceVersion
`func (o *ApplicationVersionCreateRequest) UnsetSourceVersion()`

UnsetSourceVersion ensures that no value is present for SourceVersion, not even an explicit nil
### GetComment

`func (o *ApplicationVersionCreateRequest) GetComment() string`

GetComment returns the Comment field if non-nil, zero value otherwise.

### GetCommentOk

`func (o *ApplicationVersionCreateRequest) GetCommentOk() (*string, bool)`

GetCommentOk returns a tuple with the Comment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetComment

`func (o *ApplicationVersionCreateRequest) SetComment(v string)`

SetComment sets Comment field to given value.

### HasComment

`func (o *ApplicationVersionCreateRequest) HasComment() bool`

HasComment returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


