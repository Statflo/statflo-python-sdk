# NotificationLogCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer_id** | **int** |  | [optional] 
**user_id** | **int** |  | 
**payload** | **object** |  | 
**channel** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**record_source** | **str** |  | [optional] 
**entity** | **str** |  | [optional] 
**entity_id** | **object** |  | [optional] 
**external_id** | **str** |  | [optional] 
**delivered_at** | **datetime** |  | [optional] 
**created_at** | **datetime** |  | 

## Example

```python
from statflo_python_sdk.models.notification_log_create import NotificationLogCreate

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationLogCreate from a JSON string
notification_log_create_instance = NotificationLogCreate.from_json(json)
# print the JSON string representation of the object
print(NotificationLogCreate.to_json())

# convert the object into a dict
notification_log_create_dict = notification_log_create_instance.to_dict()
# create an instance of NotificationLogCreate from a dict
notification_log_create_from_dict = NotificationLogCreate.from_dict(notification_log_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


