# ReleaseLastError

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Operation** | **string** | * &#x60;archive&#x60; - archive | 
**FromState** | **string** | * &#x60;draft&#x60; - draft * &#x60;queued&#x60; - queued * &#x60;building&#x60; - building * &#x60;ready&#x60; - ready * &#x60;error&#x60; - error * &#x60;canceled&#x60; - canceled * &#x60;archiving&#x60; - archiving * &#x60;archived&#x60; - archived * &#x60;deleting&#x60; - deleting * &#x60;deleted&#x60; - deleted | 
**Code** | **string** | Class of the failure, such as &#x60;internal&#x60;. | 
**Message** | **string** | Description of the failure. | 
**Timestamp** | **time.Time** |  | 

## Methods

### NewReleaseLastError

`func NewReleaseLastError(operation string, fromState string, code string, message string, timestamp time.Time, ) *ReleaseLastError`

NewReleaseLastError instantiates a new ReleaseLastError object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReleaseLastErrorWithDefaults

`func NewReleaseLastErrorWithDefaults() *ReleaseLastError`

NewReleaseLastErrorWithDefaults instantiates a new ReleaseLastError object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOperation

`func (o *ReleaseLastError) GetOperation() string`

GetOperation returns the Operation field if non-nil, zero value otherwise.

### GetOperationOk

`func (o *ReleaseLastError) GetOperationOk() (*string, bool)`

GetOperationOk returns a tuple with the Operation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperation

`func (o *ReleaseLastError) SetOperation(v string)`

SetOperation sets Operation field to given value.


### GetFromState

`func (o *ReleaseLastError) GetFromState() string`

GetFromState returns the FromState field if non-nil, zero value otherwise.

### GetFromStateOk

`func (o *ReleaseLastError) GetFromStateOk() (*string, bool)`

GetFromStateOk returns a tuple with the FromState field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFromState

`func (o *ReleaseLastError) SetFromState(v string)`

SetFromState sets FromState field to given value.


### GetCode

`func (o *ReleaseLastError) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *ReleaseLastError) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *ReleaseLastError) SetCode(v string)`

SetCode sets Code field to given value.


### GetMessage

`func (o *ReleaseLastError) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *ReleaseLastError) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *ReleaseLastError) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetTimestamp

`func (o *ReleaseLastError) GetTimestamp() time.Time`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *ReleaseLastError) GetTimestampOk() (*time.Time, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *ReleaseLastError) SetTimestamp(v time.Time)`

SetTimestamp sets Timestamp field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


