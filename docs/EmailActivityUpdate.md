# EmailActivityUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_content** | **str** |  | [optional] 
**message_to** | **str** |  | [optional] 
**message_from** | **str** |  | [optional] 
**subject** | **str** |  | [optional] 
**action_taken** | **str** |  | [optional] 
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
from statflo_python_sdk.models.email_activity_update import EmailActivityUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of EmailActivityUpdate from a JSON string
email_activity_update_instance = EmailActivityUpdate.from_json(json)
# print the JSON string representation of the object
print(EmailActivityUpdate.to_json())

# convert the object into a dict
email_activity_update_dict = email_activity_update_instance.to_dict()
# create an instance of EmailActivityUpdate from a dict
email_activity_update_from_dict = EmailActivityUpdate.from_dict(email_activity_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


