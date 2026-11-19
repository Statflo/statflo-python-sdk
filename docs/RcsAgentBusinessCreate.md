# RcsAgentBusinessCreate


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
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.rcs_agent_business_create import RcsAgentBusinessCreate

# TODO update the JSON string below
json = "{}"
# create an instance of RcsAgentBusinessCreate from a JSON string
rcs_agent_business_create_instance = RcsAgentBusinessCreate.from_json(json)
# print the JSON string representation of the object
print(RcsAgentBusinessCreate.to_json())

# convert the object into a dict
rcs_agent_business_create_dict = rcs_agent_business_create_instance.to_dict()
# create an instance of RcsAgentBusinessCreate from a dict
rcs_agent_business_create_from_dict = RcsAgentBusinessCreate.from_dict(rcs_agent_business_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


