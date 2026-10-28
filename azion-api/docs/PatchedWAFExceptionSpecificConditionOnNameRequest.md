# PatchedWAFExceptionSpecificConditionOnNameRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Match** | **string** | * &#x60;specific_body_form_field_name&#x60; - specific_body_form_field_name * &#x60;specific_http_header_name&#x60; - specific_http_header_name * &#x60;specific_query_string_name&#x60; - specific_query_string_name | 
**Name** | Pointer to **string** |  | [optional] 

## Methods

### NewPatchedWAFExceptionSpecificConditionOnNameRequest

`func NewPatchedWAFExceptionSpecificConditionOnNameRequest(match string, ) *PatchedWAFExceptionSpecificConditionOnNameRequest`

NewPatchedWAFExceptionSpecificConditionOnNameRequest instantiates a new PatchedWAFExceptionSpecificConditionOnNameRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedWAFExceptionSpecificConditionOnNameRequestWithDefaults

`func NewPatchedWAFExceptionSpecificConditionOnNameRequestWithDefaults() *PatchedWAFExceptionSpecificConditionOnNameRequest`

NewPatchedWAFExceptionSpecificConditionOnNameRequestWithDefaults instantiates a new PatchedWAFExceptionSpecificConditionOnNameRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMatch

`func (o *PatchedWAFExceptionSpecificConditionOnNameRequest) GetMatch() string`

GetMatch returns the Match field if non-nil, zero value otherwise.

### GetMatchOk

`func (o *PatchedWAFExceptionSpecificConditionOnNameRequest) GetMatchOk() (*string, bool)`

GetMatchOk returns a tuple with the Match field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatch

`func (o *PatchedWAFExceptionSpecificConditionOnNameRequest) SetMatch(v string)`

SetMatch sets Match field to given value.


### GetName

`func (o *PatchedWAFExceptionSpecificConditionOnNameRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *PatchedWAFExceptionSpecificConditionOnNameRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *PatchedWAFExceptionSpecificConditionOnNameRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *PatchedWAFExceptionSpecificConditionOnNameRequest) HasName() bool`

HasName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


