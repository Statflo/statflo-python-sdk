# EmailActivityPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[EmailActivity]**](EmailActivity.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.email_activity_pagination_response import EmailActivityPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of EmailActivityPaginationResponse from a JSON string
email_activity_pagination_response_instance = EmailActivityPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(EmailActivityPaginationResponse.to_json())

# convert the object into a dict
email_activity_pagination_response_dict = email_activity_pagination_response_instance.to_dict()
# create an instance of EmailActivityPaginationResponse from a dict
email_activity_pagination_response_from_dict = EmailActivityPaginationResponse.from_dict(email_activity_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


