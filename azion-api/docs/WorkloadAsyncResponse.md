# WorkloadAsyncResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**State** | Pointer to **string** |  | [optional] 
**Data** | [**Workload**](Workload.md) |  | 

## Methods

### NewWorkloadAsyncResponse

`func NewWorkloadAsyncResponse(data Workload, ) *WorkloadAsyncResponse`

NewWorkloadAsyncResponse instantiates a new WorkloadAsyncResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWorkloadAsyncResponseWithDefaults

`func NewWorkloadAsyncResponseWithDefaults() *WorkloadAsyncResponse`

NewWorkloadAsyncResponseWithDefaults instantiates a new WorkloadAsyncResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetState

`func (o *WorkloadAsyncResponse) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *WorkloadAsyncResponse) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *WorkloadAsyncResponse) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *WorkloadAsyncResponse) HasState() bool`

HasState returns a boolean if a field has been set.

### GetData

`func (o *WorkloadAsyncResponse) GetData() Workload`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *WorkloadAsyncResponse) GetDataOk() (*Workload, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *WorkloadAsyncResponse) SetData(v Workload)`

SetData sets Data field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


