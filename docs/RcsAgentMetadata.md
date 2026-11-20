# RcsAgentMetadata


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**rcs_agent** | [**RcsAgent**](RcsAgent.md) |  | 
**metadata** | **str** |  | 
**value** | **object** |  | [optional] 
**carrier** | [**Carrier**](Carrier.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.rcs_agent_metadata import RcsAgentMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of RcsAgentMetadata from a JSON string
rcs_agent_metadata_instance = RcsAgentMetadata.from_json(json)
# print the JSON string representation of the object
print(RcsAgentMetadata.to_json())

# convert the object into a dict
rcs_agent_metadata_dict = rcs_agent_metadata_instance.to_dict()
# create an instance of RcsAgentMetadata from a dict
rcs_agent_metadata_from_dict = RcsAgentMetadata.from_dict(rcs_agent_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


