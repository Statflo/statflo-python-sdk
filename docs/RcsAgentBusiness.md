# RcsAgentBusiness


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**industry** | **str** |  | [optional] 
**legal_name** | **str** |  | [optional] 
**entity_type** | **str** |  | [optional] 
**stock_exchange** | **str** |  | [optional] 
**stock_symbol** | **str** |  | [optional] 
**registration_number** | **str** |  | [optional] 
**registration_issuing_country_iso_code** | **str** |  | [optional] 
**carrier** | [**Carrier**](Carrier.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.rcs_agent_business import RcsAgentBusiness

# TODO update the JSON string below
json = "{}"
# create an instance of RcsAgentBusiness from a JSON string
rcs_agent_business_instance = RcsAgentBusiness.from_json(json)
# print the JSON string representation of the object
print(RcsAgentBusiness.to_json())

# convert the object into a dict
rcs_agent_business_dict = rcs_agent_business_instance.to_dict()
# create an instance of RcsAgentBusiness from a dict
rcs_agent_business_from_dict = RcsAgentBusiness.from_dict(rcs_agent_business_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


