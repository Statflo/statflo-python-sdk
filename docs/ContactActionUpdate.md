# ContactActionUpdate


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
**record_owned** | **int** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.contact_action_update import ContactActionUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of ContactActionUpdate from a JSON string
contact_action_update_instance = ContactActionUpdate.from_json(json)
# print the JSON string representation of the object
print(ContactActionUpdate.to_json())

# convert the object into a dict
contact_action_update_dict = contact_action_update_instance.to_dict()
# create an instance of ContactActionUpdate from a dict
contact_action_update_from_dict = ContactActionUpdate.from_dict(contact_action_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


