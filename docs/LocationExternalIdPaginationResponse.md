# LocationExternalIdPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[LocationExternalId]**](LocationExternalId.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.location_external_id_pagination_response import LocationExternalIdPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of LocationExternalIdPaginationResponse from a JSON string
location_external_id_pagination_response_instance = LocationExternalIdPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(LocationExternalIdPaginationResponse.to_json())

# convert the object into a dict
location_external_id_pagination_response_dict = location_external_id_pagination_response_instance.to_dict()
# create an instance of LocationExternalIdPaginationResponse from a dict
location_external_id_pagination_response_from_dict = LocationExternalIdPaginationResponse.from_dict(location_external_id_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


