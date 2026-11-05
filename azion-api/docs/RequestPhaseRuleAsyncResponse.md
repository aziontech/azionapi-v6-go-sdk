# RequestPhaseRuleAsyncResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**State** | Pointer to **string** |  | [optional] 
**Data** | [**RequestPhaseRule**](RequestPhaseRule.md) |  | 

## Methods

### NewRequestPhaseRuleAsyncResponse

`func NewRequestPhaseRuleAsyncResponse(data RequestPhaseRule, ) *RequestPhaseRuleAsyncResponse`

NewRequestPhaseRuleAsyncResponse instantiates a new RequestPhaseRuleAsyncResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRequestPhaseRuleAsyncResponseWithDefaults

`func NewRequestPhaseRuleAsyncResponseWithDefaults() *RequestPhaseRuleAsyncResponse`

NewRequestPhaseRuleAsyncResponseWithDefaults instantiates a new RequestPhaseRuleAsyncResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetState

`func (o *RequestPhaseRuleAsyncResponse) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *RequestPhaseRuleAsyncResponse) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *RequestPhaseRuleAsyncResponse) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *RequestPhaseRuleAsyncResponse) HasState() bool`

HasState returns a boolean if a field has been set.

### GetData

`func (o *RequestPhaseRuleAsyncResponse) GetData() RequestPhaseRule`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *RequestPhaseRuleAsyncResponse) GetDataOk() (*RequestPhaseRule, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *RequestPhaseRuleAsyncResponse) SetData(v RequestPhaseRule)`

SetData sets Data field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


