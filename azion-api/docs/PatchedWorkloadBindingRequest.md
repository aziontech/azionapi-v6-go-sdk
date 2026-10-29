# PatchedWorkloadBindingRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EnvironmentId** | Pointer to **string** |  | [optional] 
**DeploymentId** | Pointer to **string** |  | [optional] 
**Domains** | Pointer to [**[]PatchedWorkloadBindingRequestDomainsInner**](PatchedWorkloadBindingRequestDomainsInner.md) |  | [optional] 

## Methods

### NewPatchedWorkloadBindingRequest

`func NewPatchedWorkloadBindingRequest() *PatchedWorkloadBindingRequest`

NewPatchedWorkloadBindingRequest instantiates a new PatchedWorkloadBindingRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedWorkloadBindingRequestWithDefaults

`func NewPatchedWorkloadBindingRequestWithDefaults() *PatchedWorkloadBindingRequest`

NewPatchedWorkloadBindingRequestWithDefaults instantiates a new PatchedWorkloadBindingRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnvironmentId

`func (o *PatchedWorkloadBindingRequest) GetEnvironmentId() string`

GetEnvironmentId returns the EnvironmentId field if non-nil, zero value otherwise.

### GetEnvironmentIdOk

`func (o *PatchedWorkloadBindingRequest) GetEnvironmentIdOk() (*string, bool)`

GetEnvironmentIdOk returns a tuple with the EnvironmentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnvironmentId

`func (o *PatchedWorkloadBindingRequest) SetEnvironmentId(v string)`

SetEnvironmentId sets EnvironmentId field to given value.

### HasEnvironmentId

`func (o *PatchedWorkloadBindingRequest) HasEnvironmentId() bool`

HasEnvironmentId returns a boolean if a field has been set.

### GetDeploymentId

`func (o *PatchedWorkloadBindingRequest) GetDeploymentId() string`

GetDeploymentId returns the DeploymentId field if non-nil, zero value otherwise.

### GetDeploymentIdOk

`func (o *PatchedWorkloadBindingRequest) GetDeploymentIdOk() (*string, bool)`

GetDeploymentIdOk returns a tuple with the DeploymentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeploymentId

`func (o *PatchedWorkloadBindingRequest) SetDeploymentId(v string)`

SetDeploymentId sets DeploymentId field to given value.

### HasDeploymentId

`func (o *PatchedWorkloadBindingRequest) HasDeploymentId() bool`

HasDeploymentId returns a boolean if a field has been set.

### GetDomains

`func (o *PatchedWorkloadBindingRequest) GetDomains() []PatchedWorkloadBindingRequestDomainsInner`

GetDomains returns the Domains field if non-nil, zero value otherwise.

### GetDomainsOk

`func (o *PatchedWorkloadBindingRequest) GetDomainsOk() (*[]PatchedWorkloadBindingRequestDomainsInner, bool)`

GetDomainsOk returns a tuple with the Domains field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDomains

`func (o *PatchedWorkloadBindingRequest) SetDomains(v []PatchedWorkloadBindingRequestDomainsInner)`

SetDomains sets Domains field to given value.

### HasDomains

`func (o *PatchedWorkloadBindingRequest) HasDomains() bool`

HasDomains returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


