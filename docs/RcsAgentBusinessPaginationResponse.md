# RcsAgentBusinessPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[RcsAgentBusiness]**](RcsAgentBusiness.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.rcs_agent_business_pagination_response import RcsAgentBusinessPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of RcsAgentBusinessPaginationResponse from a JSON string
rcs_agent_business_pagination_response_instance = RcsAgentBusinessPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(RcsAgentBusinessPaginationResponse.to_json())

# convert the object into a dict
rcs_agent_business_pagination_response_dict = rcs_agent_business_pagination_response_instance.to_dict()
# create an instance of RcsAgentBusinessPaginationResponse from a dict
rcs_agent_business_pagination_response_from_dict = RcsAgentBusinessPaginationResponse.from_dict(rcs_agent_business_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


