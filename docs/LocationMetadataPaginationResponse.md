# LocationMetadataPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[LocationMetadata]**](LocationMetadata.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.location_metadata_pagination_response import LocationMetadataPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of LocationMetadataPaginationResponse from a JSON string
location_metadata_pagination_response_instance = LocationMetadataPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(LocationMetadataPaginationResponse.to_json())

# convert the object into a dict
location_metadata_pagination_response_dict = location_metadata_pagination_response_instance.to_dict()
# create an instance of LocationMetadataPaginationResponse from a dict
location_metadata_pagination_response_from_dict = LocationMetadataPaginationResponse.from_dict(location_metadata_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


