# AccountReleaseOrigin

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** | * &#x60;manual&#x60; - manual * &#x60;api&#x60; - api * &#x60;cli&#x60; - cli * &#x60;promotion&#x60; - promotion | 
**SourceEnvironmentId** | **NullableString** |  | 
**SourceReleaseId** | **NullableString** |  | 
**PromotedFrom** | **NullableString** |  | 

## Methods

### NewAccountReleaseOrigin

`func NewAccountReleaseOrigin(type_ string, sourceEnvironmentId NullableString, sourceReleaseId NullableString, promotedFrom NullableString, ) *AccountReleaseOrigin`

NewAccountReleaseOrigin instantiates a new AccountReleaseOrigin object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAccountReleaseOriginWithDefaults

`func NewAccountReleaseOriginWithDefaults() *AccountReleaseOrigin`

NewAccountReleaseOriginWithDefaults instantiates a new AccountReleaseOrigin object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *AccountReleaseOrigin) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *AccountReleaseOrigin) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *AccountReleaseOrigin) SetType(v string)`

SetType sets Type field to given value.


### GetSourceEnvironmentId

`func (o *AccountReleaseOrigin) GetSourceEnvironmentId() string`

GetSourceEnvironmentId returns the SourceEnvironmentId field if non-nil, zero value otherwise.

### GetSourceEnvironmentIdOk

`func (o *AccountReleaseOrigin) GetSourceEnvironmentIdOk() (*string, bool)`

GetSourceEnvironmentIdOk returns a tuple with the SourceEnvironmentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceEnvironmentId

`func (o *AccountReleaseOrigin) SetSourceEnvironmentId(v string)`

SetSourceEnvironmentId sets SourceEnvironmentId field to given value.


### SetSourceEnvironmentIdNil

`func (o *AccountReleaseOrigin) SetSourceEnvironmentIdNil(b bool)`

 SetSourceEnvironmentIdNil sets the value for SourceEnvironmentId to be an explicit nil

### UnsetSourceEnvironmentId
`func (o *AccountReleaseOrigin) UnsetSourceEnvironmentId()`

UnsetSourceEnvironmentId ensures that no value is present for SourceEnvironmentId, not even an explicit nil
### GetSourceReleaseId

`func (o *AccountReleaseOrigin) GetSourceReleaseId() string`

GetSourceReleaseId returns the SourceReleaseId field if non-nil, zero value otherwise.

### GetSourceReleaseIdOk

`func (o *AccountReleaseOrigin) GetSourceReleaseIdOk() (*string, bool)`

GetSourceReleaseIdOk returns a tuple with the SourceReleaseId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceReleaseId

`func (o *AccountReleaseOrigin) SetSourceReleaseId(v string)`

SetSourceReleaseId sets SourceReleaseId field to given value.


### SetSourceReleaseIdNil

`func (o *AccountReleaseOrigin) SetSourceReleaseIdNil(b bool)`

 SetSourceReleaseIdNil sets the value for SourceReleaseId to be an explicit nil

### UnsetSourceReleaseId
`func (o *AccountReleaseOrigin) UnsetSourceReleaseId()`

UnsetSourceReleaseId ensures that no value is present for SourceReleaseId, not even an explicit nil
### GetPromotedFrom

`func (o *AccountReleaseOrigin) GetPromotedFrom() string`

GetPromotedFrom returns the PromotedFrom field if non-nil, zero value otherwise.

### GetPromotedFromOk

`func (o *AccountReleaseOrigin) GetPromotedFromOk() (*string, bool)`

GetPromotedFromOk returns a tuple with the PromotedFrom field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPromotedFrom

`func (o *AccountReleaseOrigin) SetPromotedFrom(v string)`

SetPromotedFrom sets PromotedFrom field to given value.


### SetPromotedFromNil

`func (o *AccountReleaseOrigin) SetPromotedFromNil(b bool)`

 SetPromotedFromNil sets the value for PromotedFrom to be an explicit nil

### UnsetPromotedFrom
`func (o *AccountReleaseOrigin) UnsetPromotedFrom()`

UnsetPromotedFrom ensures that no value is present for PromotedFrom, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


