# RcsAgentUseCasePaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[RcsAgentUseCase]**](RcsAgentUseCase.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.rcs_agent_use_case_pagination_response import RcsAgentUseCasePaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of RcsAgentUseCasePaginationResponse from a JSON string
rcs_agent_use_case_pagination_response_instance = RcsAgentUseCasePaginationResponse.from_json(json)
# print the JSON string representation of the object
print(RcsAgentUseCasePaginationResponse.to_json())

# convert the object into a dict
rcs_agent_use_case_pagination_response_dict = rcs_agent_use_case_pagination_response_instance.to_dict()
# create an instance of RcsAgentUseCasePaginationResponse from a dict
rcs_agent_use_case_pagination_response_from_dict = RcsAgentUseCasePaginationResponse.from_dict(rcs_agent_use_case_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


