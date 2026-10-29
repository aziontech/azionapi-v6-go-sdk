# PatchedWAFExceptionConditionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Match** | **string** | * &#x60;specific_body_form_field_value&#x60; - specific_body_form_field_value * &#x60;specific_http_header_value&#x60; - specific_http_header_value * &#x60;specific_query_string_value&#x60; - specific_query_string_value | 
**Name** | Pointer to **string** |  | [optional] 
**Value** | Pointer to **string** |  | [optional] 

## Methods

### NewPatchedWAFExceptionConditionRequest

`func NewPatchedWAFExceptionConditionRequest(match string, ) *PatchedWAFExceptionConditionRequest`

NewPatchedWAFExceptionConditionRequest instantiates a new PatchedWAFExceptionConditionRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedWAFExceptionConditionRequestWithDefaults

`func NewPatchedWAFExceptionConditionRequestWithDefaults() *PatchedWAFExceptionConditionRequest`

NewPatchedWAFExceptionConditionRequestWithDefaults instantiates a new PatchedWAFExceptionConditionRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMatch

`func (o *PatchedWAFExceptionConditionRequest) GetMatch() string`

GetMatch returns the Match field if non-nil, zero value otherwise.

### GetMatchOk

`func (o *PatchedWAFExceptionConditionRequest) GetMatchOk() (*string, bool)`

GetMatchOk returns a tuple with the Match field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatch

`func (o *PatchedWAFExceptionConditionRequest) SetMatch(v string)`

SetMatch sets Match field to given value.


### GetName

`func (o *PatchedWAFExceptionConditionRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *PatchedWAFExceptionConditionRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *PatchedWAFExceptionConditionRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *PatchedWAFExceptionConditionRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### GetValue

`func (o *PatchedWAFExceptionConditionRequest) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *PatchedWAFExceptionConditionRequest) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *PatchedWAFExceptionConditionRequest) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *PatchedWAFExceptionConditionRequest) HasValue() bool`

HasValue returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


