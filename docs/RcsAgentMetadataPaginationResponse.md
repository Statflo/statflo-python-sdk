# RcsAgentMetadataPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[RcsAgentMetadata]**](RcsAgentMetadata.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.rcs_agent_metadata_pagination_response import RcsAgentMetadataPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of RcsAgentMetadataPaginationResponse from a JSON string
rcs_agent_metadata_pagination_response_instance = RcsAgentMetadataPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(RcsAgentMetadataPaginationResponse.to_json())

# convert the object into a dict
rcs_agent_metadata_pagination_response_dict = rcs_agent_metadata_pagination_response_instance.to_dict()
# create an instance of RcsAgentMetadataPaginationResponse from a dict
rcs_agent_metadata_pagination_response_from_dict = RcsAgentMetadataPaginationResponse.from_dict(rcs_agent_metadata_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


