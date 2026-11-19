# AccountMemberPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[AccountMember]**](AccountMember.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.account_member_pagination_response import AccountMemberPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AccountMemberPaginationResponse from a JSON string
account_member_pagination_response_instance = AccountMemberPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(AccountMemberPaginationResponse.to_json())

# convert the object into a dict
account_member_pagination_response_dict = account_member_pagination_response_instance.to_dict()
# create an instance of AccountMemberPaginationResponse from a dict
account_member_pagination_response_from_dict = AccountMemberPaginationResponse.from_dict(account_member_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


