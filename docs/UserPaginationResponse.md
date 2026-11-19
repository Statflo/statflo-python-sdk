# UserPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[User]**](User.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.user_pagination_response import UserPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserPaginationResponse from a JSON string
user_pagination_response_instance = UserPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(UserPaginationResponse.to_json())

# convert the object into a dict
user_pagination_response_dict = user_pagination_response_instance.to_dict()
# create an instance of UserPaginationResponse from a dict
user_pagination_response_from_dict = UserPaginationResponse.from_dict(user_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


