# PatchedWorkloadBindingRequestDomainsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Domain** | **string** |  | 
**Certificate** | Pointer to **NullableInt64** |  | [optional] 

## Methods

### NewPatchedWorkloadBindingRequestDomainsInner

`func NewPatchedWorkloadBindingRequestDomainsInner(domain string, ) *PatchedWorkloadBindingRequestDomainsInner`

NewPatchedWorkloadBindingRequestDomainsInner instantiates a new PatchedWorkloadBindingRequestDomainsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedWorkloadBindingRequestDomainsInnerWithDefaults

`func NewPatchedWorkloadBindingRequestDomainsInnerWithDefaults() *PatchedWorkloadBindingRequestDomainsInner`

NewPatchedWorkloadBindingRequestDomainsInnerWithDefaults instantiates a new PatchedWorkloadBindingRequestDomainsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDomain

`func (o *PatchedWorkloadBindingRequestDomainsInner) GetDomain() string`

GetDomain returns the Domain field if non-nil, zero value otherwise.

### GetDomainOk

`func (o *PatchedWorkloadBindingRequestDomainsInner) GetDomainOk() (*string, bool)`

GetDomainOk returns a tuple with the Domain field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDomain

`func (o *PatchedWorkloadBindingRequestDomainsInner) SetDomain(v string)`

SetDomain sets Domain field to given value.


### GetCertificate

`func (o *PatchedWorkloadBindingRequestDomainsInner) GetCertificate() int64`

GetCertificate returns the Certificate field if non-nil, zero value otherwise.

### GetCertificateOk

`func (o *PatchedWorkloadBindingRequestDomainsInner) GetCertificateOk() (*int64, bool)`

GetCertificateOk returns a tuple with the Certificate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCertificate

`func (o *PatchedWorkloadBindingRequestDomainsInner) SetCertificate(v int64)`

SetCertificate sets Certificate field to given value.

### HasCertificate

`func (o *PatchedWorkloadBindingRequestDomainsInner) HasCertificate() bool`

HasCertificate returns a boolean if a field has been set.

### SetCertificateNil

`func (o *PatchedWorkloadBindingRequestDomainsInner) SetCertificateNil(b bool)`

 SetCertificateNil sets the value for Certificate to be an explicit nil

### UnsetCertificate
`func (o *PatchedWorkloadBindingRequestDomainsInner) UnsetCertificate()`

UnsetCertificate ensures that no value is present for Certificate, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


