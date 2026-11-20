# AccountNumber


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**location** | **str** |  | [optional] 
**user** | [**User**](User.md) |  | 
**phone_number** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.account_number import AccountNumber

# TODO update the JSON string below
json = "{}"
# create an instance of AccountNumber from a JSON string
account_number_instance = AccountNumber.from_json(json)
# print the JSON string representation of the object
print(AccountNumber.to_json())

# convert the object into a dict
account_number_dict = account_number_instance.to_dict()
# create an instance of AccountNumber from a dict
account_number_from_dict = AccountNumber.from_dict(account_number_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


