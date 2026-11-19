# WidgetPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Widget]**](Widget.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.widget_pagination_response import WidgetPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WidgetPaginationResponse from a JSON string
widget_pagination_response_instance = WidgetPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(WidgetPaginationResponse.to_json())

# convert the object into a dict
widget_pagination_response_dict = widget_pagination_response_instance.to_dict()
# create an instance of WidgetPaginationResponse from a dict
widget_pagination_response_from_dict = WidgetPaginationResponse.from_dict(widget_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


