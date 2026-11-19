# LocationPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Location]**](Location.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.location_pagination_response import LocationPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of LocationPaginationResponse from a JSON string
location_pagination_response_instance = LocationPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(LocationPaginationResponse.to_json())

# convert the object into a dict
location_pagination_response_dict = location_pagination_response_instance.to_dict()
# create an instance of LocationPaginationResponse from a dict
location_pagination_response_from_dict = LocationPaginationResponse.from_dict(location_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


