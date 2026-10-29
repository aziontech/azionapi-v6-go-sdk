# PatchedWAFExceptionSpecificConditionOnValueRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Match** | **string** | * &#x60;specific_body_form_field_value&#x60; - specific_body_form_field_value * &#x60;specific_http_header_value&#x60; - specific_http_header_value * &#x60;specific_query_string_value&#x60; - specific_query_string_value | 
**Value** | Pointer to **string** |  | [optional] 

## Methods

### NewPatchedWAFExceptionSpecificConditionOnValueRequest

`func NewPatchedWAFExceptionSpecificConditionOnValueRequest(match string, ) *PatchedWAFExceptionSpecificConditionOnValueRequest`

NewPatchedWAFExceptionSpecificConditionOnValueRequest instantiates a new PatchedWAFExceptionSpecificConditionOnValueRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedWAFExceptionSpecificConditionOnValueRequestWithDefaults

`func NewPatchedWAFExceptionSpecificConditionOnValueRequestWithDefaults() *PatchedWAFExceptionSpecificConditionOnValueRequest`

NewPatchedWAFExceptionSpecificConditionOnValueRequestWithDefaults instantiates a new PatchedWAFExceptionSpecificConditionOnValueRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMatch

`func (o *PatchedWAFExceptionSpecificConditionOnValueRequest) GetMatch() string`

GetMatch returns the Match field if non-nil, zero value otherwise.

### GetMatchOk

`func (o *PatchedWAFExceptionSpecificConditionOnValueRequest) GetMatchOk() (*string, bool)`

GetMatchOk returns a tuple with the Match field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatch

`func (o *PatchedWAFExceptionSpecificConditionOnValueRequest) SetMatch(v string)`

SetMatch sets Match field to given value.


### GetValue

`func (o *PatchedWAFExceptionSpecificConditionOnValueRequest) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *PatchedWAFExceptionSpecificConditionOnValueRequest) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *PatchedWAFExceptionSpecificConditionOnValueRequest) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *PatchedWAFExceptionSpecificConditionOnValueRequest) HasValue() bool`

HasValue returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


