# CallActivity


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**call_to** | **str** |  | [optional] 
**content** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**action_taken** | **str** |  | [optional] 
**next_steps** | **str** |  | [optional] 
**next_date** | **datetime** |  | [optional] 
**call_outcome** | **str** |  | [optional] 
**outcome_location** | **str** |  | [optional] 
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
from statflo_python_sdk.models.call_activity import CallActivity

# TODO update the JSON string below
json = "{}"
# create an instance of CallActivity from a JSON string
call_activity_instance = CallActivity.from_json(json)
# print the JSON string representation of the object
print(CallActivity.to_json())

# convert the object into a dict
call_activity_dict = call_activity_instance.to_dict()
# create an instance of CallActivity from a dict
call_activity_from_dict = CallActivity.from_dict(call_activity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


