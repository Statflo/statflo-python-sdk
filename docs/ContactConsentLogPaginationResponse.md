# ContactConsentLogPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[ContactConsentLog]**](ContactConsentLog.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.contact_consent_log_pagination_response import ContactConsentLogPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ContactConsentLogPaginationResponse from a JSON string
contact_consent_log_pagination_response_instance = ContactConsentLogPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(ContactConsentLogPaginationResponse.to_json())

# convert the object into a dict
contact_consent_log_pagination_response_dict = contact_consent_log_pagination_response_instance.to_dict()
# create an instance of ContactConsentLogPaginationResponse from a dict
contact_consent_log_pagination_response_from_dict = ContactConsentLogPaginationResponse.from_dict(contact_consent_log_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


