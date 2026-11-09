# CustomPageVersionCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Pages** | Pointer to [**[]PageRequest**](PageRequest.md) |  | [optional] 
**SourceVersion** | Pointer to **NullableString** | ID of the version to clone from. If omitted, clones latest ready. | [optional] 
**Comment** | Pointer to **string** | Accepted and not stored. | [optional] 

## Methods

### NewCustomPageVersionCreateRequest

`func NewCustomPageVersionCreateRequest() *CustomPageVersionCreateRequest`

NewCustomPageVersionCreateRequest instantiates a new CustomPageVersionCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCustomPageVersionCreateRequestWithDefaults

`func NewCustomPageVersionCreateRequestWithDefaults() *CustomPageVersionCreateRequest`

NewCustomPageVersionCreateRequestWithDefaults instantiates a new CustomPageVersionCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CustomPageVersionCreateRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CustomPageVersionCreateRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CustomPageVersionCreateRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *CustomPageVersionCreateRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetPages

`func (o *CustomPageVersionCreateRequest) GetPages() []PageRequest`

GetPages returns the Pages field if non-nil, zero value otherwise.

### GetPagesOk

`func (o *CustomPageVersionCreateRequest) GetPagesOk() (*[]PageRequest, bool)`

GetPagesOk returns a tuple with the Pages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPages

`func (o *CustomPageVersionCreateRequest) SetPages(v []PageRequest)`

SetPages sets Pages field to given value.

### HasPages

`func (o *CustomPageVersionCreateRequest) HasPages() bool`

HasPages returns a boolean if a field has been set.

### GetSourceVersion

`func (o *CustomPageVersionCreateRequest) GetSourceVersion() string`

GetSourceVersion returns the SourceVersion field if non-nil, zero value otherwise.

### GetSourceVersionOk

`func (o *CustomPageVersionCreateRequest) GetSourceVersionOk() (*string, bool)`

GetSourceVersionOk returns a tuple with the SourceVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceVersion

`func (o *CustomPageVersionCreateRequest) SetSourceVersion(v string)`

SetSourceVersion sets SourceVersion field to given value.

### HasSourceVersion

`func (o *CustomPageVersionCreateRequest) HasSourceVersion() bool`

HasSourceVersion returns a boolean if a field has been set.

### SetSourceVersionNil

`func (o *CustomPageVersionCreateRequest) SetSourceVersionNil(b bool)`

 SetSourceVersionNil sets the value for SourceVersion to be an explicit nil

### UnsetSourceVersion
`func (o *CustomPageVersionCreateRequest) UnsetSourceVersion()`

UnsetSourceVersion ensures that no value is present for SourceVersion, not even an explicit nil
### GetComment

`func (o *CustomPageVersionCreateRequest) GetComment() string`

GetComment returns the Comment field if non-nil, zero value otherwise.

### GetCommentOk

`func (o *CustomPageVersionCreateRequest) GetCommentOk() (*string, bool)`

GetCommentOk returns a tuple with the Comment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetComment

`func (o *CustomPageVersionCreateRequest) SetComment(v string)`

SetComment sets Comment field to given value.

### HasComment

`func (o *CustomPageVersionCreateRequest) HasComment() bool`

HasComment returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


