# PatchedPageConnectorAttributesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Connector** | Pointer to **int32** |  | [optional] 
**Ttl** | Pointer to **int32** |  | [optional] 
**Uri** | Pointer to **NullableString** |  | [optional] 
**CustomStatusCode** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewPatchedPageConnectorAttributesRequest

`func NewPatchedPageConnectorAttributesRequest() *PatchedPageConnectorAttributesRequest`

NewPatchedPageConnectorAttributesRequest instantiates a new PatchedPageConnectorAttributesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedPageConnectorAttributesRequestWithDefaults

`func NewPatchedPageConnectorAttributesRequestWithDefaults() *PatchedPageConnectorAttributesRequest`

NewPatchedPageConnectorAttributesRequestWithDefaults instantiates a new PatchedPageConnectorAttributesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetConnector

`func (o *PatchedPageConnectorAttributesRequest) GetConnector() int32`

GetConnector returns the Connector field if non-nil, zero value otherwise.

### GetConnectorOk

`func (o *PatchedPageConnectorAttributesRequest) GetConnectorOk() (*int32, bool)`

GetConnectorOk returns a tuple with the Connector field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnector

`func (o *PatchedPageConnectorAttributesRequest) SetConnector(v int32)`

SetConnector sets Connector field to given value.

### HasConnector

`func (o *PatchedPageConnectorAttributesRequest) HasConnector() bool`

HasConnector returns a boolean if a field has been set.

### GetTtl

`func (o *PatchedPageConnectorAttributesRequest) GetTtl() int32`

GetTtl returns the Ttl field if non-nil, zero value otherwise.

### GetTtlOk

`func (o *PatchedPageConnectorAttributesRequest) GetTtlOk() (*int32, bool)`

GetTtlOk returns a tuple with the Ttl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTtl

`func (o *PatchedPageConnectorAttributesRequest) SetTtl(v int32)`

SetTtl sets Ttl field to given value.

### HasTtl

`func (o *PatchedPageConnectorAttributesRequest) HasTtl() bool`

HasTtl returns a boolean if a field has been set.

### GetUri

`func (o *PatchedPageConnectorAttributesRequest) GetUri() string`

GetUri returns the Uri field if non-nil, zero value otherwise.

### GetUriOk

`func (o *PatchedPageConnectorAttributesRequest) GetUriOk() (*string, bool)`

GetUriOk returns a tuple with the Uri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUri

`func (o *PatchedPageConnectorAttributesRequest) SetUri(v string)`

SetUri sets Uri field to given value.

### HasUri

`func (o *PatchedPageConnectorAttributesRequest) HasUri() bool`

HasUri returns a boolean if a field has been set.

### SetUriNil

`func (o *PatchedPageConnectorAttributesRequest) SetUriNil(b bool)`

 SetUriNil sets the value for Uri to be an explicit nil

### UnsetUri
`func (o *PatchedPageConnectorAttributesRequest) UnsetUri()`

UnsetUri ensures that no value is present for Uri, not even an explicit nil
### GetCustomStatusCode

`func (o *PatchedPageConnectorAttributesRequest) GetCustomStatusCode() int32`

GetCustomStatusCode returns the CustomStatusCode field if non-nil, zero value otherwise.

### GetCustomStatusCodeOk

`func (o *PatchedPageConnectorAttributesRequest) GetCustomStatusCodeOk() (*int32, bool)`

GetCustomStatusCodeOk returns a tuple with the CustomStatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomStatusCode

`func (o *PatchedPageConnectorAttributesRequest) SetCustomStatusCode(v int32)`

SetCustomStatusCode sets CustomStatusCode field to given value.

### HasCustomStatusCode

`func (o *PatchedPageConnectorAttributesRequest) HasCustomStatusCode() bool`

HasCustomStatusCode returns a boolean if a field has been set.

### SetCustomStatusCodeNil

`func (o *PatchedPageConnectorAttributesRequest) SetCustomStatusCodeNil(b bool)`

 SetCustomStatusCodeNil sets the value for CustomStatusCode to be an explicit nil

### UnsetCustomStatusCode
`func (o *PatchedPageConnectorAttributesRequest) UnsetCustomStatusCode()`

UnsetCustomStatusCode ensures that no value is present for CustomStatusCode, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


