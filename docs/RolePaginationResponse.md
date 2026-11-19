# RolePaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Role]**](Role.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.role_pagination_response import RolePaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of RolePaginationResponse from a JSON string
role_pagination_response_instance = RolePaginationResponse.from_json(json)
# print the JSON string representation of the object
print(RolePaginationResponse.to_json())

# convert the object into a dict
role_pagination_response_dict = role_pagination_response_instance.to_dict()
# create an instance of RolePaginationResponse from a dict
role_pagination_response_from_dict = RolePaginationResponse.from_dict(role_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


