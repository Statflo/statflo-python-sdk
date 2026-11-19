# LocationFallbackUserPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[LocationFallbackUser]**](LocationFallbackUser.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.location_fallback_user_pagination_response import LocationFallbackUserPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of LocationFallbackUserPaginationResponse from a JSON string
location_fallback_user_pagination_response_instance = LocationFallbackUserPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(LocationFallbackUserPaginationResponse.to_json())

# convert the object into a dict
location_fallback_user_pagination_response_dict = location_fallback_user_pagination_response_instance.to_dict()
# create an instance of LocationFallbackUserPaginationResponse from a dict
location_fallback_user_pagination_response_from_dict = LocationFallbackUserPaginationResponse.from_dict(location_fallback_user_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


