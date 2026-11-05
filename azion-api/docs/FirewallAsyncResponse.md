# FirewallAsyncResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**State** | Pointer to **string** |  | [optional] 
**Data** | [**Firewall**](Firewall.md) |  | 

## Methods

### NewFirewallAsyncResponse

`func NewFirewallAsyncResponse(data Firewall, ) *FirewallAsyncResponse`

NewFirewallAsyncResponse instantiates a new FirewallAsyncResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFirewallAsyncResponseWithDefaults

`func NewFirewallAsyncResponseWithDefaults() *FirewallAsyncResponse`

NewFirewallAsyncResponseWithDefaults instantiates a new FirewallAsyncResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetState

`func (o *FirewallAsyncResponse) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *FirewallAsyncResponse) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *FirewallAsyncResponse) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *FirewallAsyncResponse) HasState() bool`

HasState returns a boolean if a field has been set.

### GetData

`func (o *FirewallAsyncResponse) GetData() Firewall`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *FirewallAsyncResponse) GetDataOk() (*Firewall, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *FirewallAsyncResponse) SetData(v Firewall)`

SetData sets Data field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


