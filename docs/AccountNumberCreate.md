# AccountNumberCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**location** | **str** |  | [optional] 
**user_id** | **int** |  | 
**phone_number** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.account_number_create import AccountNumberCreate

# TODO update the JSON string below
json = "{}"
# create an instance of AccountNumberCreate from a JSON string
account_number_create_instance = AccountNumberCreate.from_json(json)
# print the JSON string representation of the object
print(AccountNumberCreate.to_json())

# convert the object into a dict
account_number_create_dict = account_number_create_instance.to_dict()
# create an instance of AccountNumberCreate from a dict
account_number_create_from_dict = AccountNumberCreate.from_dict(account_number_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


