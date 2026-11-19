# Timeline


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
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
from statflo_python_sdk.models.timeline import Timeline

# TODO update the JSON string below
json = "{}"
# create an instance of Timeline from a JSON string
timeline_instance = Timeline.from_json(json)
# print the JSON string representation of the object
print(Timeline.to_json())

# convert the object into a dict
timeline_dict = timeline_instance.to_dict()
# create an instance of Timeline from a dict
timeline_from_dict = Timeline.from_dict(timeline_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


