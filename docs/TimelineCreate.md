# TimelineCreate


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
**record_owned** | **int** |  | [optional] [default to 1]

## Example

```python
from statflo_python_sdk.models.timeline_create import TimelineCreate

# TODO update the JSON string below
json = "{}"
# create an instance of TimelineCreate from a JSON string
timeline_create_instance = TimelineCreate.from_json(json)
# print the JSON string representation of the object
print(TimelineCreate.to_json())

# convert the object into a dict
timeline_create_dict = timeline_create_instance.to_dict()
# create an instance of TimelineCreate from a dict
timeline_create_from_dict = TimelineCreate.from_dict(timeline_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


