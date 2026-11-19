# BulkMessagePaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[BulkMessage]**](BulkMessage.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.bulk_message_pagination_response import BulkMessagePaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BulkMessagePaginationResponse from a JSON string
bulk_message_pagination_response_instance = BulkMessagePaginationResponse.from_json(json)
# print the JSON string representation of the object
print(BulkMessagePaginationResponse.to_json())

# convert the object into a dict
bulk_message_pagination_response_dict = bulk_message_pagination_response_instance.to_dict()
# create an instance of BulkMessagePaginationResponse from a dict
bulk_message_pagination_response_from_dict = BulkMessagePaginationResponse.from_dict(bulk_message_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


