# NotepadPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Notepad]**](Notepad.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.notepad_pagination_response import NotepadPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of NotepadPaginationResponse from a JSON string
notepad_pagination_response_instance = NotepadPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(NotepadPaginationResponse.to_json())

# convert the object into a dict
notepad_pagination_response_dict = notepad_pagination_response_instance.to_dict()
# create an instance of NotepadPaginationResponse from a dict
notepad_pagination_response_from_dict = NotepadPaginationResponse.from_dict(notepad_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


