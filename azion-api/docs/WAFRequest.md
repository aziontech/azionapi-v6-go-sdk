# WAFRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**EngineSettings** | Pointer to [**WAFEngineSettingsFieldRequest**](WAFEngineSettingsFieldRequest.md) |  | [optional] 

## Methods

### NewWAFRequest

`func NewWAFRequest(name string, ) *WAFRequest`

NewWAFRequest instantiates a new WAFRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWAFRequestWithDefaults

`func NewWAFRequestWithDefaults() *WAFRequest`

NewWAFRequestWithDefaults instantiates a new WAFRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *WAFRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *WAFRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *WAFRequest) SetName(v string)`

SetName sets Name field to given value.


### GetEngineSettings

`func (o *WAFRequest) GetEngineSettings() WAFEngineSettingsFieldRequest`

GetEngineSettings returns the EngineSettings field if non-nil, zero value otherwise.

### GetEngineSettingsOk

`func (o *WAFRequest) GetEngineSettingsOk() (*WAFEngineSettingsFieldRequest, bool)`

GetEngineSettingsOk returns a tuple with the EngineSettings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEngineSettings

`func (o *WAFRequest) SetEngineSettings(v WAFEngineSettingsFieldRequest)`

SetEngineSettings sets EngineSettings field to given value.

### HasEngineSettings

`func (o *WAFRequest) HasEngineSettings() bool`

HasEngineSettings returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


