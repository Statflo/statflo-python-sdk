# WidgetMetadataUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**widget_id** | **int** |  | [optional] 
**metadata** | **str** |  | 
**value** | **object** |  | 

## Example

```python
from statflo_python_sdk.models.widget_metadata_update import WidgetMetadataUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of WidgetMetadataUpdate from a JSON string
widget_metadata_update_instance = WidgetMetadataUpdate.from_json(json)
# print the JSON string representation of the object
print(WidgetMetadataUpdate.to_json())

# convert the object into a dict
widget_metadata_update_dict = widget_metadata_update_instance.to_dict()
# create an instance of WidgetMetadataUpdate from a dict
widget_metadata_update_from_dict = WidgetMetadataUpdate.from_dict(widget_metadata_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


