# RegionPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Region]**](Region.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.region_pagination_response import RegionPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of RegionPaginationResponse from a JSON string
region_pagination_response_instance = RegionPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(RegionPaginationResponse.to_json())

# convert the object into a dict
region_pagination_response_dict = region_pagination_response_instance.to_dict()
# create an instance of RegionPaginationResponse from a dict
region_pagination_response_from_dict = RegionPaginationResponse.from_dict(region_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


