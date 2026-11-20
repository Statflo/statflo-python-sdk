# NotepadUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**action_taken** | **str** |  | [optional] 
**id** | **int** |  | 
**type** | **int** |  | 
**account_id** | **str** |  | 
**date_added** | **datetime** |  | 
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | 
**record_source** | **str** |  | [optional] 
**record_owned** | **int** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.notepad_update import NotepadUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of NotepadUpdate from a JSON string
notepad_update_instance = NotepadUpdate.from_json(json)
# print the JSON string representation of the object
print(NotepadUpdate.to_json())

# convert the object into a dict
notepad_update_dict = notepad_update_instance.to_dict()
# create an instance of NotepadUpdate from a dict
notepad_update_from_dict = NotepadUpdate.from_dict(notepad_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


