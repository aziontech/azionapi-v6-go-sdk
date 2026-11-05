# ConnectorVersionCreateRequestAttributes

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Addresses** | [**[]AddressRequest**](AddressRequest.md) |  | 
**ConnectionOptions** | Pointer to [**HTTPConnectionOptionsRequest**](HTTPConnectionOptionsRequest.md) |  | [optional] 
**Modules** | Pointer to [**HTTPModulesRequest**](HTTPModulesRequest.md) |  | [optional] 
**Bucket** | **string** |  | 
**Prefix** | Pointer to **string** |  | [optional] 
**Region** | **string** | * &#x60;us-east-1&#x60; - us-east-1 * &#x60;us-east-2&#x60; - us-east-2 * &#x60;br-east-1&#x60; - br-east-1 * &#x60;br-east-2&#x60; - br-east-2 * &#x60;br-east-3&#x60; - br-east-3 | 

## Methods

### NewConnectorVersionCreateRequestAttributes

`func NewConnectorVersionCreateRequestAttributes(addresses []AddressRequest, bucket string, region string, ) *ConnectorVersionCreateRequestAttributes`

NewConnectorVersionCreateRequestAttributes instantiates a new ConnectorVersionCreateRequestAttributes object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConnectorVersionCreateRequestAttributesWithDefaults

`func NewConnectorVersionCreateRequestAttributesWithDefaults() *ConnectorVersionCreateRequestAttributes`

NewConnectorVersionCreateRequestAttributesWithDefaults instantiates a new ConnectorVersionCreateRequestAttributes object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAddresses

`func (o *ConnectorVersionCreateRequestAttributes) GetAddresses() []AddressRequest`

GetAddresses returns the Addresses field if non-nil, zero value otherwise.

### GetAddressesOk

`func (o *ConnectorVersionCreateRequestAttributes) GetAddressesOk() (*[]AddressRequest, bool)`

GetAddressesOk returns a tuple with the Addresses field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAddresses

`func (o *ConnectorVersionCreateRequestAttributes) SetAddresses(v []AddressRequest)`

SetAddresses sets Addresses field to given value.


### GetConnectionOptions

`func (o *ConnectorVersionCreateRequestAttributes) GetConnectionOptions() HTTPConnectionOptionsRequest`

GetConnectionOptions returns the ConnectionOptions field if non-nil, zero value otherwise.

### GetConnectionOptionsOk

`func (o *ConnectorVersionCreateRequestAttributes) GetConnectionOptionsOk() (*HTTPConnectionOptionsRequest, bool)`

GetConnectionOptionsOk returns a tuple with the ConnectionOptions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnectionOptions

`func (o *ConnectorVersionCreateRequestAttributes) SetConnectionOptions(v HTTPConnectionOptionsRequest)`

SetConnectionOptions sets ConnectionOptions field to given value.

### HasConnectionOptions

`func (o *ConnectorVersionCreateRequestAttributes) HasConnectionOptions() bool`

HasConnectionOptions returns a boolean if a field has been set.

### GetModules

`func (o *ConnectorVersionCreateRequestAttributes) GetModules() HTTPModulesRequest`

GetModules returns the Modules field if non-nil, zero value otherwise.

### GetModulesOk

`func (o *ConnectorVersionCreateRequestAttributes) GetModulesOk() (*HTTPModulesRequest, bool)`

GetModulesOk returns a tuple with the Modules field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModules

`func (o *ConnectorVersionCreateRequestAttributes) SetModules(v HTTPModulesRequest)`

SetModules sets Modules field to given value.

### HasModules

`func (o *ConnectorVersionCreateRequestAttributes) HasModules() bool`

HasModules returns a boolean if a field has been set.

### GetBucket

`func (o *ConnectorVersionCreateRequestAttributes) GetBucket() string`

GetBucket returns the Bucket field if non-nil, zero value otherwise.

### GetBucketOk

`func (o *ConnectorVersionCreateRequestAttributes) GetBucketOk() (*string, bool)`

GetBucketOk returns a tuple with the Bucket field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBucket

`func (o *ConnectorVersionCreateRequestAttributes) SetBucket(v string)`

SetBucket sets Bucket field to given value.


### GetPrefix

`func (o *ConnectorVersionCreateRequestAttributes) GetPrefix() string`

GetPrefix returns the Prefix field if non-nil, zero value otherwise.

### GetPrefixOk

`func (o *ConnectorVersionCreateRequestAttributes) GetPrefixOk() (*string, bool)`

GetPrefixOk returns a tuple with the Prefix field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrefix

`func (o *ConnectorVersionCreateRequestAttributes) SetPrefix(v string)`

SetPrefix sets Prefix field to given value.

### HasPrefix

`func (o *ConnectorVersionCreateRequestAttributes) HasPrefix() bool`

HasPrefix returns a boolean if a field has been set.

### GetRegion

`func (o *ConnectorVersionCreateRequestAttributes) GetRegion() string`

GetRegion returns the Region field if non-nil, zero value otherwise.

### GetRegionOk

`func (o *ConnectorVersionCreateRequestAttributes) GetRegionOk() (*string, bool)`

GetRegionOk returns a tuple with the Region field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegion

`func (o *ConnectorVersionCreateRequestAttributes) SetRegion(v string)`

SetRegion sets Region field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


