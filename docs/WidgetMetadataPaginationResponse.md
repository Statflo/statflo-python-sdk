# WidgetMetadataPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[WidgetMetadata]**](WidgetMetadata.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.widget_metadata_pagination_response import WidgetMetadataPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WidgetMetadataPaginationResponse from a JSON string
widget_metadata_pagination_response_instance = WidgetMetadataPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(WidgetMetadataPaginationResponse.to_json())

# convert the object into a dict
widget_metadata_pagination_response_dict = widget_metadata_pagination_response_instance.to_dict()
# create an instance of WidgetMetadataPaginationResponse from a dict
widget_metadata_pagination_response_from_dict = WidgetMetadataPaginationResponse.from_dict(widget_metadata_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


