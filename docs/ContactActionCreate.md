# ContactActionCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_content** | **str** |  | [optional] 
**message_to** | **str** |  | [optional] 
**message_from** | **str** |  | [optional] 
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
from statflo_python_sdk.models.contact_action_create import ContactActionCreate

# TODO update the JSON string below
json = "{}"
# create an instance of ContactActionCreate from a JSON string
contact_action_create_instance = ContactActionCreate.from_json(json)
# print the JSON string representation of the object
print(ContactActionCreate.to_json())

# convert the object into a dict
contact_action_create_dict = contact_action_create_instance.to_dict()
# create an instance of ContactActionCreate from a dict
contact_action_create_from_dict = ContactActionCreate.from_dict(contact_action_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


