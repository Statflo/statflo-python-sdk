# WidgetMetadataCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**widget_id** | **int** |  | 
**metadata** | **str** |  | 
**value** | **object** |  | 

## Example

```python
from statflo_python_sdk.models.widget_metadata_create import WidgetMetadataCreate

# TODO update the JSON string below
json = "{}"
# create an instance of WidgetMetadataCreate from a JSON string
widget_metadata_create_instance = WidgetMetadataCreate.from_json(json)
# print the JSON string representation of the object
print(WidgetMetadataCreate.to_json())

# convert the object into a dict
widget_metadata_create_dict = widget_metadata_create_instance.to_dict()
# create an instance of WidgetMetadataCreate from a dict
widget_metadata_create_from_dict = WidgetMetadataCreate.from_dict(widget_metadata_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


