# AccountContactMetadataPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[AccountContactMetadata]**](AccountContactMetadata.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.account_contact_metadata_pagination_response import AccountContactMetadataPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AccountContactMetadataPaginationResponse from a JSON string
account_contact_metadata_pagination_response_instance = AccountContactMetadataPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(AccountContactMetadataPaginationResponse.to_json())

# convert the object into a dict
account_contact_metadata_pagination_response_dict = account_contact_metadata_pagination_response_instance.to_dict()
# create an instance of AccountContactMetadataPaginationResponse from a dict
account_contact_metadata_pagination_response_from_dict = AccountContactMetadataPaginationResponse.from_dict(account_contact_metadata_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


