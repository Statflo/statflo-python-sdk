# NotificationLogPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[NotificationLog]**](NotificationLog.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.notification_log_pagination_response import NotificationLogPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationLogPaginationResponse from a JSON string
notification_log_pagination_response_instance = NotificationLogPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(NotificationLogPaginationResponse.to_json())

# convert the object into a dict
notification_log_pagination_response_dict = notification_log_pagination_response_instance.to_dict()
# create an instance of NotificationLogPaginationResponse from a dict
notification_log_pagination_response_from_dict = NotificationLogPaginationResponse.from_dict(notification_log_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


