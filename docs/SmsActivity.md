# SmsActivity


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
**message_template** | [**MessageTemplate**](MessageTemplate.md) |  | 
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
from statflo_python_sdk.models.sms_activity import SmsActivity

# TODO update the JSON string below
json = "{}"
# create an instance of SmsActivity from a JSON string
sms_activity_instance = SmsActivity.from_json(json)
# print the JSON string representation of the object
print(SmsActivity.to_json())

# convert the object into a dict
sms_activity_dict = sms_activity_instance.to_dict()
# create an instance of SmsActivity from a dict
sms_activity_from_dict = SmsActivity.from_dict(sms_activity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


