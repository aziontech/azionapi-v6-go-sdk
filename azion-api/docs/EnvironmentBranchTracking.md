# EnvironmentBranchTracking

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | **bool** |  | 
**Mode** | **string** | * &#x60;branch_is&#x60; - branch_is * &#x60;branch_starts_with&#x60; - branch_starts_with * &#x60;branch_ends_with&#x60; - branch_ends_with | 
**BranchMatch** | **string** |  | 

## Methods

### NewEnvironmentBranchTracking

`func NewEnvironmentBranchTracking(enabled bool, mode string, branchMatch string, ) *EnvironmentBranchTracking`

NewEnvironmentBranchTracking instantiates a new EnvironmentBranchTracking object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEnvironmentBranchTrackingWithDefaults

`func NewEnvironmentBranchTrackingWithDefaults() *EnvironmentBranchTracking`

NewEnvironmentBranchTrackingWithDefaults instantiates a new EnvironmentBranchTracking object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *EnvironmentBranchTracking) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *EnvironmentBranchTracking) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *EnvironmentBranchTracking) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.


### GetMode

`func (o *EnvironmentBranchTracking) GetMode() string`

GetMode returns the Mode field if non-nil, zero value otherwise.

### GetModeOk

`func (o *EnvironmentBranchTracking) GetModeOk() (*string, bool)`

GetModeOk returns a tuple with the Mode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMode

`func (o *EnvironmentBranchTracking) SetMode(v string)`

SetMode sets Mode field to given value.


### GetBranchMatch

`func (o *EnvironmentBranchTracking) GetBranchMatch() string`

GetBranchMatch returns the BranchMatch field if non-nil, zero value otherwise.

### GetBranchMatchOk

`func (o *EnvironmentBranchTracking) GetBranchMatchOk() (*string, bool)`

GetBranchMatchOk returns a tuple with the BranchMatch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBranchMatch

`func (o *EnvironmentBranchTracking) SetBranchMatch(v string)`

SetBranchMatch sets BranchMatch field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


