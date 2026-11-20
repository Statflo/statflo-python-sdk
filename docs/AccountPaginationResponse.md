# AccountPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Account]**](Account.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.account_pagination_response import AccountPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AccountPaginationResponse from a JSON string
account_pagination_response_instance = AccountPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(AccountPaginationResponse.to_json())

# convert the object into a dict
account_pagination_response_dict = account_pagination_response_instance.to_dict()
# create an instance of AccountPaginationResponse from a dict
account_pagination_response_from_dict = AccountPaginationResponse.from_dict(account_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


