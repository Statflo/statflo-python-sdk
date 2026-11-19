# SmsActivityCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | 
**assigned_to** | **str** |  | 
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
**record_owned** | **int** |  | [optional] [default to 1]

## Example

```python
from statflo_python_sdk.models.sms_activity_create import SmsActivityCreate

# TODO update the JSON string below
json = "{}"
# create an instance of SmsActivityCreate from a JSON string
sms_activity_create_instance = SmsActivityCreate.from_json(json)
# print the JSON string representation of the object
print(SmsActivityCreate.to_json())

# convert the object into a dict
sms_activity_create_dict = sms_activity_create_instance.to_dict()
# create an instance of SmsActivityCreate from a dict
sms_activity_create_from_dict = SmsActivityCreate.from_dict(sms_activity_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


