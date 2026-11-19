# SmsActivityUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | 
**assigned_to** | **str** |  | [optional] 
**assigned_from** | **str** |  | [optional] 
**action_taken** | **str** |  | [optional] 
**subject** | **str** |  | [optional] 
**source_id** | **str** |  | [optional] 
**next_steps** | **str** |  | [optional] 
**next_date** | **datetime** |  | [optional] 
**outcome_reason** | **str** |  | [optional] 
**message_template_id** | **str** |  | [optional] 
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
from statflo_python_sdk.models.sms_activity_update import SmsActivityUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of SmsActivityUpdate from a JSON string
sms_activity_update_instance = SmsActivityUpdate.from_json(json)
# print the JSON string representation of the object
print(SmsActivityUpdate.to_json())

# convert the object into a dict
sms_activity_update_dict = sms_activity_update_instance.to_dict()
# create an instance of SmsActivityUpdate from a dict
sms_activity_update_from_dict = SmsActivityUpdate.from_dict(sms_activity_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


