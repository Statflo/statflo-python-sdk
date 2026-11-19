# NotepadCreate


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
**record_owned** | **int** |  | [optional] [default to 1]

## Example

```python
from statflo_python_sdk.models.notepad_create import NotepadCreate

# TODO update the JSON string below
json = "{}"
# create an instance of NotepadCreate from a JSON string
notepad_create_instance = NotepadCreate.from_json(json)
# print the JSON string representation of the object
print(NotepadCreate.to_json())

# convert the object into a dict
notepad_create_dict = notepad_create_instance.to_dict()
# create an instance of NotepadCreate from a dict
notepad_create_from_dict = NotepadCreate.from_dict(notepad_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


