# PatchedHttpProtocolRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Versions** | Pointer to **[]string** |  | [optional] 
**HttpPorts** | Pointer to **[]int64** |  | [optional] 
**HttpsPorts** | Pointer to **[]int64** |  | [optional] 
**QuicPorts** | Pointer to **[]int64** |  | [optional] 

## Methods

### NewPatchedHttpProtocolRequest

`func NewPatchedHttpProtocolRequest() *PatchedHttpProtocolRequest`

NewPatchedHttpProtocolRequest instantiates a new PatchedHttpProtocolRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedHttpProtocolRequestWithDefaults

`func NewPatchedHttpProtocolRequestWithDefaults() *PatchedHttpProtocolRequest`

NewPatchedHttpProtocolRequestWithDefaults instantiates a new PatchedHttpProtocolRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersions

`func (o *PatchedHttpProtocolRequest) GetVersions() []string`

GetVersions returns the Versions field if non-nil, zero value otherwise.

### GetVersionsOk

`func (o *PatchedHttpProtocolRequest) GetVersionsOk() (*[]string, bool)`

GetVersionsOk returns a tuple with the Versions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersions

`func (o *PatchedHttpProtocolRequest) SetVersions(v []string)`

SetVersions sets Versions field to given value.

### HasVersions

`func (o *PatchedHttpProtocolRequest) HasVersions() bool`

HasVersions returns a boolean if a field has been set.

### GetHttpPorts

`func (o *PatchedHttpProtocolRequest) GetHttpPorts() []int64`

GetHttpPorts returns the HttpPorts field if non-nil, zero value otherwise.

### GetHttpPortsOk

`func (o *PatchedHttpProtocolRequest) GetHttpPortsOk() (*[]int64, bool)`

GetHttpPortsOk returns a tuple with the HttpPorts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpPorts

`func (o *PatchedHttpProtocolRequest) SetHttpPorts(v []int64)`

SetHttpPorts sets HttpPorts field to given value.

### HasHttpPorts

`func (o *PatchedHttpProtocolRequest) HasHttpPorts() bool`

HasHttpPorts returns a boolean if a field has been set.

### GetHttpsPorts

`func (o *PatchedHttpProtocolRequest) GetHttpsPorts() []int64`

GetHttpsPorts returns the HttpsPorts field if non-nil, zero value otherwise.

### GetHttpsPortsOk

`func (o *PatchedHttpProtocolRequest) GetHttpsPortsOk() (*[]int64, bool)`

GetHttpsPortsOk returns a tuple with the HttpsPorts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpsPorts

`func (o *PatchedHttpProtocolRequest) SetHttpsPorts(v []int64)`

SetHttpsPorts sets HttpsPorts field to given value.

### HasHttpsPorts

`func (o *PatchedHttpProtocolRequest) HasHttpsPorts() bool`

HasHttpsPorts returns a boolean if a field has been set.

### SetHttpsPortsNil

`func (o *PatchedHttpProtocolRequest) SetHttpsPortsNil(b bool)`

 SetHttpsPortsNil sets the value for HttpsPorts to be an explicit nil

### UnsetHttpsPorts
`func (o *PatchedHttpProtocolRequest) UnsetHttpsPorts()`

UnsetHttpsPorts ensures that no value is present for HttpsPorts, not even an explicit nil
### GetQuicPorts

`func (o *PatchedHttpProtocolRequest) GetQuicPorts() []int64`

GetQuicPorts returns the QuicPorts field if non-nil, zero value otherwise.

### GetQuicPortsOk

`func (o *PatchedHttpProtocolRequest) GetQuicPortsOk() (*[]int64, bool)`

GetQuicPortsOk returns a tuple with the QuicPorts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuicPorts

`func (o *PatchedHttpProtocolRequest) SetQuicPorts(v []int64)`

SetQuicPorts sets QuicPorts field to given value.

### HasQuicPorts

`func (o *PatchedHttpProtocolRequest) HasQuicPorts() bool`

HasQuicPorts returns a boolean if a field has been set.

### SetQuicPortsNil

`func (o *PatchedHttpProtocolRequest) SetQuicPortsNil(b bool)`

 SetQuicPortsNil sets the value for QuicPorts to be an explicit nil

### UnsetQuicPorts
`func (o *PatchedHttpProtocolRequest) UnsetQuicPorts()`

UnsetQuicPorts ensures that no value is present for QuicPorts, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


