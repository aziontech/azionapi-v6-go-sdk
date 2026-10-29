# ResourceHierarchyResponseDataResources

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Application** | [**NullableResourceHierarchyResponseDataResourcesApplication**](ResourceHierarchyResponseDataResourcesApplication.md) |  | 
**Firewall** | [**NullableResourceHierarchyResponseDataResourcesApplication**](ResourceHierarchyResponseDataResourcesApplication.md) |  | 
**CustomPage** | [**NullableResourceHierarchyResponseDataResourcesApplication**](ResourceHierarchyResponseDataResourcesApplication.md) |  | 
**Waf** | [**[]ResourceHierarchyResponseDataResourcesWafInner**](ResourceHierarchyResponseDataResourcesWafInner.md) |  | 
**Function** | [**[]ResourceHierarchyResponseDataResourcesWafInner**](ResourceHierarchyResponseDataResourcesWafInner.md) |  | 
**Connector** | [**[]ResourceHierarchyResponseDataResourcesWafInner**](ResourceHierarchyResponseDataResourcesWafInner.md) |  | 
**NetworkList** | [**[]ResourceHierarchyResponseDataResourcesWafInner**](ResourceHierarchyResponseDataResourcesWafInner.md) |  | 

## Methods

### NewResourceHierarchyResponseDataResources

`func NewResourceHierarchyResponseDataResources(application NullableResourceHierarchyResponseDataResourcesApplication, firewall NullableResourceHierarchyResponseDataResourcesApplication, customPage NullableResourceHierarchyResponseDataResourcesApplication, waf []ResourceHierarchyResponseDataResourcesWafInner, function []ResourceHierarchyResponseDataResourcesWafInner, connector []ResourceHierarchyResponseDataResourcesWafInner, networkList []ResourceHierarchyResponseDataResourcesWafInner, ) *ResourceHierarchyResponseDataResources`

NewResourceHierarchyResponseDataResources instantiates a new ResourceHierarchyResponseDataResources object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResourceHierarchyResponseDataResourcesWithDefaults

`func NewResourceHierarchyResponseDataResourcesWithDefaults() *ResourceHierarchyResponseDataResources`

NewResourceHierarchyResponseDataResourcesWithDefaults instantiates a new ResourceHierarchyResponseDataResources object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetApplication

`func (o *ResourceHierarchyResponseDataResources) GetApplication() ResourceHierarchyResponseDataResourcesApplication`

GetApplication returns the Application field if non-nil, zero value otherwise.

### GetApplicationOk

`func (o *ResourceHierarchyResponseDataResources) GetApplicationOk() (*ResourceHierarchyResponseDataResourcesApplication, bool)`

GetApplicationOk returns a tuple with the Application field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApplication

`func (o *ResourceHierarchyResponseDataResources) SetApplication(v ResourceHierarchyResponseDataResourcesApplication)`

SetApplication sets Application field to given value.


### SetApplicationNil

`func (o *ResourceHierarchyResponseDataResources) SetApplicationNil(b bool)`

 SetApplicationNil sets the value for Application to be an explicit nil

### UnsetApplication
`func (o *ResourceHierarchyResponseDataResources) UnsetApplication()`

UnsetApplication ensures that no value is present for Application, not even an explicit nil
### GetFirewall

`func (o *ResourceHierarchyResponseDataResources) GetFirewall() ResourceHierarchyResponseDataResourcesApplication`

GetFirewall returns the Firewall field if non-nil, zero value otherwise.

### GetFirewallOk

`func (o *ResourceHierarchyResponseDataResources) GetFirewallOk() (*ResourceHierarchyResponseDataResourcesApplication, bool)`

GetFirewallOk returns a tuple with the Firewall field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirewall

`func (o *ResourceHierarchyResponseDataResources) SetFirewall(v ResourceHierarchyResponseDataResourcesApplication)`

SetFirewall sets Firewall field to given value.


### SetFirewallNil

`func (o *ResourceHierarchyResponseDataResources) SetFirewallNil(b bool)`

 SetFirewallNil sets the value for Firewall to be an explicit nil

### UnsetFirewall
`func (o *ResourceHierarchyResponseDataResources) UnsetFirewall()`

UnsetFirewall ensures that no value is present for Firewall, not even an explicit nil
### GetCustomPage

`func (o *ResourceHierarchyResponseDataResources) GetCustomPage() ResourceHierarchyResponseDataResourcesApplication`

GetCustomPage returns the CustomPage field if non-nil, zero value otherwise.

### GetCustomPageOk

`func (o *ResourceHierarchyResponseDataResources) GetCustomPageOk() (*ResourceHierarchyResponseDataResourcesApplication, bool)`

GetCustomPageOk returns a tuple with the CustomPage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomPage

`func (o *ResourceHierarchyResponseDataResources) SetCustomPage(v ResourceHierarchyResponseDataResourcesApplication)`

SetCustomPage sets CustomPage field to given value.


### SetCustomPageNil

`func (o *ResourceHierarchyResponseDataResources) SetCustomPageNil(b bool)`

 SetCustomPageNil sets the value for CustomPage to be an explicit nil

### UnsetCustomPage
`func (o *ResourceHierarchyResponseDataResources) UnsetCustomPage()`

UnsetCustomPage ensures that no value is present for CustomPage, not even an explicit nil
### GetWaf

`func (o *ResourceHierarchyResponseDataResources) GetWaf() []ResourceHierarchyResponseDataResourcesWafInner`

GetWaf returns the Waf field if non-nil, zero value otherwise.

### GetWafOk

`func (o *ResourceHierarchyResponseDataResources) GetWafOk() (*[]ResourceHierarchyResponseDataResourcesWafInner, bool)`

GetWafOk returns a tuple with the Waf field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWaf

`func (o *ResourceHierarchyResponseDataResources) SetWaf(v []ResourceHierarchyResponseDataResourcesWafInner)`

SetWaf sets Waf field to given value.


### GetFunction

`func (o *ResourceHierarchyResponseDataResources) GetFunction() []ResourceHierarchyResponseDataResourcesWafInner`

GetFunction returns the Function field if non-nil, zero value otherwise.

### GetFunctionOk

`func (o *ResourceHierarchyResponseDataResources) GetFunctionOk() (*[]ResourceHierarchyResponseDataResourcesWafInner, bool)`

GetFunctionOk returns a tuple with the Function field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFunction

`func (o *ResourceHierarchyResponseDataResources) SetFunction(v []ResourceHierarchyResponseDataResourcesWafInner)`

SetFunction sets Function field to given value.


### GetConnector

`func (o *ResourceHierarchyResponseDataResources) GetConnector() []ResourceHierarchyResponseDataResourcesWafInner`

GetConnector returns the Connector field if non-nil, zero value otherwise.

### GetConnectorOk

`func (o *ResourceHierarchyResponseDataResources) GetConnectorOk() (*[]ResourceHierarchyResponseDataResourcesWafInner, bool)`

GetConnectorOk returns a tuple with the Connector field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnector

`func (o *ResourceHierarchyResponseDataResources) SetConnector(v []ResourceHierarchyResponseDataResourcesWafInner)`

SetConnector sets Connector field to given value.


### GetNetworkList

`func (o *ResourceHierarchyResponseDataResources) GetNetworkList() []ResourceHierarchyResponseDataResourcesWafInner`

GetNetworkList returns the NetworkList field if non-nil, zero value otherwise.

### GetNetworkListOk

`func (o *ResourceHierarchyResponseDataResources) GetNetworkListOk() (*[]ResourceHierarchyResponseDataResourcesWafInner, bool)`

GetNetworkListOk returns a tuple with the NetworkList field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNetworkList

`func (o *ResourceHierarchyResponseDataResources) SetNetworkList(v []ResourceHierarchyResponseDataResourcesWafInner)`

SetNetworkList sets NetworkList field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


