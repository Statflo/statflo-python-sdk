# WidgetCreate


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
**priority** | **int** |  | [optional] [default to 0]
**native_remote** | **str** |  | [optional] 
**native_module** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.widget_create import WidgetCreate

# TODO update the JSON string below
json = "{}"
# create an instance of WidgetCreate from a JSON string
widget_create_instance = WidgetCreate.from_json(json)
# print the JSON string representation of the object
print(WidgetCreate.to_json())

# convert the object into a dict
widget_create_dict = widget_create_instance.to_dict()
# create an instance of WidgetCreate from a dict
widget_create_from_dict = WidgetCreate.from_dict(widget_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


