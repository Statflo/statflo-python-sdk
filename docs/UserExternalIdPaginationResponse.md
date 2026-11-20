# UserExternalIdPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[UserExternalId]**](UserExternalId.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.user_external_id_pagination_response import UserExternalIdPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserExternalIdPaginationResponse from a JSON string
user_external_id_pagination_response_instance = UserExternalIdPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(UserExternalIdPaginationResponse.to_json())

# convert the object into a dict
user_external_id_pagination_response_dict = user_external_id_pagination_response_instance.to_dict()
# create an instance of UserExternalIdPaginationResponse from a dict
user_external_id_pagination_response_from_dict = UserExternalIdPaginationResponse.from_dict(user_external_id_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


