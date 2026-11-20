# DistrictPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[District]**](District.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.district_pagination_response import DistrictPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DistrictPaginationResponse from a JSON string
district_pagination_response_instance = DistrictPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(DistrictPaginationResponse.to_json())

# convert the object into a dict
district_pagination_response_dict = district_pagination_response_instance.to_dict()
# create an instance of DistrictPaginationResponse from a dict
district_pagination_response_from_dict = DistrictPaginationResponse.from_dict(district_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


