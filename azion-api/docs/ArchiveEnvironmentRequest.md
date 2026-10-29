# ArchiveEnvironmentRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Reason** | **string** | * &#x60;SUPERSEDED&#x60; - SUPERSEDED * &#x60;SECURITY_ISSUE&#x60; - SECURITY_ISSUE * &#x60;POLICY_VIOLATION&#x60; - POLICY_VIOLATION * &#x60;MANUAL&#x60; - MANUAL | 
**Comment** | Pointer to **string** |  | [optional] 

## Methods

### NewArchiveEnvironmentRequest

`func NewArchiveEnvironmentRequest(reason string, ) *ArchiveEnvironmentRequest`

NewArchiveEnvironmentRequest instantiates a new ArchiveEnvironmentRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewArchiveEnvironmentRequestWithDefaults

`func NewArchiveEnvironmentRequestWithDefaults() *ArchiveEnvironmentRequest`

NewArchiveEnvironmentRequestWithDefaults instantiates a new ArchiveEnvironmentRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetReason

`func (o *ArchiveEnvironmentRequest) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *ArchiveEnvironmentRequest) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *ArchiveEnvironmentRequest) SetReason(v string)`

SetReason sets Reason field to given value.


### GetComment

`func (o *ArchiveEnvironmentRequest) GetComment() string`

GetComment returns the Comment field if non-nil, zero value otherwise.

### GetCommentOk

`func (o *ArchiveEnvironmentRequest) GetCommentOk() (*string, bool)`

GetCommentOk returns a tuple with the Comment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetComment

`func (o *ArchiveEnvironmentRequest) SetComment(v string)`

SetComment sets Comment field to given value.

### HasComment

`func (o *ArchiveEnvironmentRequest) HasComment() bool`

HasComment returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


