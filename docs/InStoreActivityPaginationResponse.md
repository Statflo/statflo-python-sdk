# InStoreActivityPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[InStoreActivity]**](InStoreActivity.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.in_store_activity_pagination_response import InStoreActivityPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InStoreActivityPaginationResponse from a JSON string
in_store_activity_pagination_response_instance = InStoreActivityPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(InStoreActivityPaginationResponse.to_json())

# convert the object into a dict
in_store_activity_pagination_response_dict = in_store_activity_pagination_response_instance.to_dict()
# create an instance of InStoreActivityPaginationResponse from a dict
in_store_activity_pagination_response_from_dict = InStoreActivityPaginationResponse.from_dict(in_store_activity_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


