# ContactActionPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[ContactAction]**](ContactAction.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.contact_action_pagination_response import ContactActionPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ContactActionPaginationResponse from a JSON string
contact_action_pagination_response_instance = ContactActionPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(ContactActionPaginationResponse.to_json())

# convert the object into a dict
contact_action_pagination_response_dict = contact_action_pagination_response_instance.to_dict()
# create an instance of ContactActionPaginationResponse from a dict
contact_action_pagination_response_from_dict = ContactActionPaginationResponse.from_dict(contact_action_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


