# ReleaseAsyncResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**State** | **string** | * &#x60;draft&#x60; - draft * &#x60;queued&#x60; - queued * &#x60;building&#x60; - building * &#x60;ready&#x60; - ready * &#x60;error&#x60; - error * &#x60;canceled&#x60; - canceled * &#x60;archiving&#x60; - archiving * &#x60;archived&#x60; - archived * &#x60;deleting&#x60; - deleting * &#x60;deleted&#x60; - deleted | 
**TraceId** | Pointer to **string** |  | [optional] 

## Methods

### NewReleaseAsyncResponseData

`func NewReleaseAsyncResponseData(id string, state string, ) *ReleaseAsyncResponseData`

NewReleaseAsyncResponseData instantiates a new ReleaseAsyncResponseData object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReleaseAsyncResponseDataWithDefaults

`func NewReleaseAsyncResponseDataWithDefaults() *ReleaseAsyncResponseData`

NewReleaseAsyncResponseDataWithDefaults instantiates a new ReleaseAsyncResponseData object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ReleaseAsyncResponseData) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ReleaseAsyncResponseData) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ReleaseAsyncResponseData) SetId(v string)`

SetId sets Id field to given value.


### GetState

`func (o *ReleaseAsyncResponseData) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *ReleaseAsyncResponseData) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *ReleaseAsyncResponseData) SetState(v string)`

SetState sets State field to given value.


### GetTraceId

`func (o *ReleaseAsyncResponseData) GetTraceId() string`

GetTraceId returns the TraceId field if non-nil, zero value otherwise.

### GetTraceIdOk

`func (o *ReleaseAsyncResponseData) GetTraceIdOk() (*string, bool)`

GetTraceIdOk returns a tuple with the TraceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTraceId

`func (o *ReleaseAsyncResponseData) SetTraceId(v string)`

SetTraceId sets TraceId field to given value.

### HasTraceId

`func (o *ReleaseAsyncResponseData) HasTraceId() bool`

HasTraceId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


