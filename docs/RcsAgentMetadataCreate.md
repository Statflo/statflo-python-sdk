# RcsAgentMetadataCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**rcs_agent_id** | **int** |  | 
**metadata** | **str** |  | 
**value** | **object** |  | [optional] 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.rcs_agent_metadata_create import RcsAgentMetadataCreate

# TODO update the JSON string below
json = "{}"
# create an instance of RcsAgentMetadataCreate from a JSON string
rcs_agent_metadata_create_instance = RcsAgentMetadataCreate.from_json(json)
# print the JSON string representation of the object
print(RcsAgentMetadataCreate.to_json())

# convert the object into a dict
rcs_agent_metadata_create_dict = rcs_agent_metadata_create_instance.to_dict()
# create an instance of RcsAgentMetadataCreate from a dict
rcs_agent_metadata_create_from_dict = RcsAgentMetadataCreate.from_dict(rcs_agent_metadata_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


