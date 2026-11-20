# TeamPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Team]**](Team.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.team_pagination_response import TeamPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TeamPaginationResponse from a JSON string
team_pagination_response_instance = TeamPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(TeamPaginationResponse.to_json())

# convert the object into a dict
team_pagination_response_dict = team_pagination_response_instance.to_dict()
# create an instance of TeamPaginationResponse from a dict
team_pagination_response_from_dict = TeamPaginationResponse.from_dict(team_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


