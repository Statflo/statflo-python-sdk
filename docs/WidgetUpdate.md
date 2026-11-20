# WidgetUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**carrier_id** | **int** |  | [optional] 
**dealer_id** | **int** |  | [optional] 
**name** | **str** |  | 
**label** | **str** |  | [optional] 
**url** | **str** |  | 
**type** | **str** |  | 
**priority** | **int** |  | [optional] 
**native_remote** | **str** |  | [optional] 
**native_module** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.widget_update import WidgetUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of WidgetUpdate from a JSON string
widget_update_instance = WidgetUpdate.from_json(json)
# print the JSON string representation of the object
print(WidgetUpdate.to_json())

# convert the object into a dict
widget_update_dict = widget_update_instance.to_dict()
# create an instance of WidgetUpdate from a dict
widget_update_from_dict = WidgetUpdate.from_dict(widget_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


