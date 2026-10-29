# PatchedOriginShieldConfigRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OriginIpAcl** | Pointer to [**PatchedOriginIPACLRequest**](PatchedOriginIPACLRequest.md) |  | [optional] 
**Hmac** | Pointer to [**PatchedHMACRequest**](PatchedHMACRequest.md) |  | [optional] 

## Methods

### NewPatchedOriginShieldConfigRequest

`func NewPatchedOriginShieldConfigRequest() *PatchedOriginShieldConfigRequest`

NewPatchedOriginShieldConfigRequest instantiates a new PatchedOriginShieldConfigRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchedOriginShieldConfigRequestWithDefaults

`func NewPatchedOriginShieldConfigRequestWithDefaults() *PatchedOriginShieldConfigRequest`

NewPatchedOriginShieldConfigRequestWithDefaults instantiates a new PatchedOriginShieldConfigRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOriginIpAcl

`func (o *PatchedOriginShieldConfigRequest) GetOriginIpAcl() PatchedOriginIPACLRequest`

GetOriginIpAcl returns the OriginIpAcl field if non-nil, zero value otherwise.

### GetOriginIpAclOk

`func (o *PatchedOriginShieldConfigRequest) GetOriginIpAclOk() (*PatchedOriginIPACLRequest, bool)`

GetOriginIpAclOk returns a tuple with the OriginIpAcl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginIpAcl

`func (o *PatchedOriginShieldConfigRequest) SetOriginIpAcl(v PatchedOriginIPACLRequest)`

SetOriginIpAcl sets OriginIpAcl field to given value.

### HasOriginIpAcl

`func (o *PatchedOriginShieldConfigRequest) HasOriginIpAcl() bool`

HasOriginIpAcl returns a boolean if a field has been set.

### GetHmac

`func (o *PatchedOriginShieldConfigRequest) GetHmac() PatchedHMACRequest`

GetHmac returns the Hmac field if non-nil, zero value otherwise.

### GetHmacOk

`func (o *PatchedOriginShieldConfigRequest) GetHmacOk() (*PatchedHMACRequest, bool)`

GetHmacOk returns a tuple with the Hmac field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHmac

`func (o *PatchedOriginShieldConfigRequest) SetHmac(v PatchedHMACRequest)`

SetHmac sets Hmac field to given value.

### HasHmac

`func (o *PatchedOriginShieldConfigRequest) HasHmac() bool`

HasHmac returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


