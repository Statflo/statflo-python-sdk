# ContactPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Contact]**](Contact.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.contact_pagination_response import ContactPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ContactPaginationResponse from a JSON string
contact_pagination_response_instance = ContactPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(ContactPaginationResponse.to_json())

# convert the object into a dict
contact_pagination_response_dict = contact_pagination_response_instance.to_dict()
# create an instance of ContactPaginationResponse from a dict
contact_pagination_response_from_dict = ContactPaginationResponse.from_dict(contact_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


