# Notepad


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**action_taken** | **str** |  | [optional] 
**id** | **int** |  | 
**type** | **int** |  | 
**user** | [**User**](User.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**account_id** | **str** |  | 
**date_added** | **datetime** |  | 
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | 
**record_source** | **str** |  | [optional] 
**record_owned** | **int** |  | [optional] [default to 1]

## Example

```python
from statflo_python_sdk.models.notepad import Notepad

# TODO update the JSON string below
json = "{}"
# create an instance of Notepad from a JSON string
notepad_instance = Notepad.from_json(json)
# print the JSON string representation of the object
print(Notepad.to_json())

# convert the object into a dict
notepad_dict = notepad_instance.to_dict()
# create an instance of Notepad from a dict
notepad_from_dict = Notepad.from_dict(notepad_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


