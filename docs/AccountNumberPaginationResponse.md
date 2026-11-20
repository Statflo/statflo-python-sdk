# AccountNumberPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[AccountNumber]**](AccountNumber.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.account_number_pagination_response import AccountNumberPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AccountNumberPaginationResponse from a JSON string
account_number_pagination_response_instance = AccountNumberPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(AccountNumberPaginationResponse.to_json())

# convert the object into a dict
account_number_pagination_response_dict = account_number_pagination_response_instance.to_dict()
# create an instance of AccountNumberPaginationResponse from a dict
account_number_pagination_response_from_dict = AccountNumberPaginationResponse.from_dict(account_number_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


