# NotificationLog


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**carrier** | [**Carrier**](Carrier.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**user** | [**User**](User.md) |  | 
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
from statflo_python_sdk.models.notification_log import NotificationLog

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationLog from a JSON string
notification_log_instance = NotificationLog.from_json(json)
# print the JSON string representation of the object
print(NotificationLog.to_json())

# convert the object into a dict
notification_log_dict = notification_log_instance.to_dict()
# create an instance of NotificationLog from a dict
notification_log_from_dict = NotificationLog.from_dict(notification_log_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


