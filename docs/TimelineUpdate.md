# TimelineUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
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
from statflo_python_sdk.models.timeline_update import TimelineUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of TimelineUpdate from a JSON string
timeline_update_instance = TimelineUpdate.from_json(json)
# print the JSON string representation of the object
print(TimelineUpdate.to_json())

# convert the object into a dict
timeline_update_dict = timeline_update_instance.to_dict()
# create an instance of TimelineUpdate from a dict
timeline_update_from_dict = TimelineUpdate.from_dict(timeline_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


