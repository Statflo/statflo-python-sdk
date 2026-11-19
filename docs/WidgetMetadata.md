# WidgetMetadata


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**widget** | [**Widget**](Widget.md) |  | 
**metadata** | **str** |  | 
**value** | **object** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.widget_metadata import WidgetMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of WidgetMetadata from a JSON string
widget_metadata_instance = WidgetMetadata.from_json(json)
# print the JSON string representation of the object
print(WidgetMetadata.to_json())

# convert the object into a dict
widget_metadata_dict = widget_metadata_instance.to_dict()
# create an instance of WidgetMetadata from a dict
widget_metadata_from_dict = WidgetMetadata.from_dict(widget_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


