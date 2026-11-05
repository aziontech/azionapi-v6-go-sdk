# ConnectorVersionCreateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Active** | Pointer to **bool** |  | [optional] 
**Type** | Pointer to **string** | The connector&#39;s current type. Optional, and no other type is accepted. | [optional] 
**Attributes** | Pointer to [**ConnectorVersionCreateRequestAttributes**](ConnectorVersionCreateRequestAttributes.md) |  | [optional] 
**SourceVersion** | Pointer to **NullableString** | ID of the version to clone from. If omitted, clones latest ready. | [optional] 
**Comment** | Pointer to **string** | Accepted and not stored. | [optional] 

## Methods

### NewConnectorVersionCreateRequest

`func NewConnectorVersionCreateRequest() *ConnectorVersionCreateRequest`

NewConnectorVersionCreateRequest instantiates a new ConnectorVersionCreateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConnectorVersionCreateRequestWithDefaults

`func NewConnectorVersionCreateRequestWithDefaults() *ConnectorVersionCreateRequest`

NewConnectorVersionCreateRequestWithDefaults instantiates a new ConnectorVersionCreateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *ConnectorVersionCreateRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ConnectorVersionCreateRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ConnectorVersionCreateRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ConnectorVersionCreateRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetActive

`func (o *ConnectorVersionCreateRequest) GetActive() bool`

GetActive returns the Active field if non-nil, zero value otherwise.

### GetActiveOk

`func (o *ConnectorVersionCreateRequest) GetActiveOk() (*bool, bool)`

GetActiveOk returns a tuple with the Active field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActive

`func (o *ConnectorVersionCreateRequest) SetActive(v bool)`

SetActive sets Active field to given value.

### HasActive

`func (o *ConnectorVersionCreateRequest) HasActive() bool`

HasActive returns a boolean if a field has been set.

### GetType

`func (o *ConnectorVersionCreateRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ConnectorVersionCreateRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ConnectorVersionCreateRequest) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ConnectorVersionCreateRequest) HasType() bool`

HasType returns a boolean if a field has been set.

### GetAttributes

`func (o *ConnectorVersionCreateRequest) GetAttributes() ConnectorVersionCreateRequestAttributes`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *ConnectorVersionCreateRequest) GetAttributesOk() (*ConnectorVersionCreateRequestAttributes, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *ConnectorVersionCreateRequest) SetAttributes(v ConnectorVersionCreateRequestAttributes)`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *ConnectorVersionCreateRequest) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.

### GetSourceVersion

`func (o *ConnectorVersionCreateRequest) GetSourceVersion() string`

GetSourceVersion returns the SourceVersion field if non-nil, zero value otherwise.

### GetSourceVersionOk

`func (o *ConnectorVersionCreateRequest) GetSourceVersionOk() (*string, bool)`

GetSourceVersionOk returns a tuple with the SourceVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceVersion

`func (o *ConnectorVersionCreateRequest) SetSourceVersion(v string)`

SetSourceVersion sets SourceVersion field to given value.

### HasSourceVersion

`func (o *ConnectorVersionCreateRequest) HasSourceVersion() bool`

HasSourceVersion returns a boolean if a field has been set.

### SetSourceVersionNil

`func (o *ConnectorVersionCreateRequest) SetSourceVersionNil(b bool)`

 SetSourceVersionNil sets the value for SourceVersion to be an explicit nil

### UnsetSourceVersion
`func (o *ConnectorVersionCreateRequest) UnsetSourceVersion()`

UnsetSourceVersion ensures that no value is present for SourceVersion, not even an explicit nil
### GetComment

`func (o *ConnectorVersionCreateRequest) GetComment() string`

GetComment returns the Comment field if non-nil, zero value otherwise.

### GetCommentOk

`func (o *ConnectorVersionCreateRequest) GetCommentOk() (*string, bool)`

GetCommentOk returns a tuple with the Comment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetComment

`func (o *ConnectorVersionCreateRequest) SetComment(v string)`

SetComment sets Comment field to given value.

### HasComment

`func (o *ConnectorVersionCreateRequest) HasComment() bool`

HasComment returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


