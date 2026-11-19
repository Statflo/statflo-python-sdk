# EmailActivityCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_content** | **str** |  | 
**message_to** | **str** |  | 
**message_from** | **str** |  | [optional] [default to 'none']
**subject** | **str** |  | [optional] 
**action_taken** | **str** |  | [optional] [default to 'none']
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
from statflo_python_sdk.models.email_activity_create import EmailActivityCreate

# TODO update the JSON string below
json = "{}"
# create an instance of EmailActivityCreate from a JSON string
email_activity_create_instance = EmailActivityCreate.from_json(json)
# print the JSON string representation of the object
print(EmailActivityCreate.to_json())

# convert the object into a dict
email_activity_create_dict = email_activity_create_instance.to_dict()
# create an instance of EmailActivityCreate from a dict
email_activity_create_from_dict = EmailActivityCreate.from_dict(email_activity_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


