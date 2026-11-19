# RcsAgentMetadataUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**rcs_agent_id** | **int** |  | [optional] 
**metadata** | **str** |  | 
**value** | **object** |  | [optional] 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.rcs_agent_metadata_update import RcsAgentMetadataUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of RcsAgentMetadataUpdate from a JSON string
rcs_agent_metadata_update_instance = RcsAgentMetadataUpdate.from_json(json)
# print the JSON string representation of the object
print(RcsAgentMetadataUpdate.to_json())

# convert the object into a dict
rcs_agent_metadata_update_dict = rcs_agent_metadata_update_instance.to_dict()
# create an instance of RcsAgentMetadataUpdate from a dict
rcs_agent_metadata_update_from_dict = RcsAgentMetadataUpdate.from_dict(rcs_agent_metadata_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


