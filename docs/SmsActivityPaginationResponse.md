# SmsActivityPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[SmsActivity]**](SmsActivity.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.sms_activity_pagination_response import SmsActivityPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SmsActivityPaginationResponse from a JSON string
sms_activity_pagination_response_instance = SmsActivityPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(SmsActivityPaginationResponse.to_json())

# convert the object into a dict
sms_activity_pagination_response_dict = sms_activity_pagination_response_instance.to_dict()
# create an instance of SmsActivityPaginationResponse from a dict
sms_activity_pagination_response_from_dict = SmsActivityPaginationResponse.from_dict(sms_activity_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


