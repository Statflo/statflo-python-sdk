# CallActivityPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[CallActivity]**](CallActivity.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.call_activity_pagination_response import CallActivityPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CallActivityPaginationResponse from a JSON string
call_activity_pagination_response_instance = CallActivityPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(CallActivityPaginationResponse.to_json())

# convert the object into a dict
call_activity_pagination_response_dict = call_activity_pagination_response_instance.to_dict()
# create an instance of CallActivityPaginationResponse from a dict
call_activity_pagination_response_from_dict = CallActivityPaginationResponse.from_dict(call_activity_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


