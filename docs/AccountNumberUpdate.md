# AccountNumberUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**location** | **str** |  | [optional] 
**user_id** | **int** |  | 
**phone_number** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.account_number_update import AccountNumberUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of AccountNumberUpdate from a JSON string
account_number_update_instance = AccountNumberUpdate.from_json(json)
# print the JSON string representation of the object
print(AccountNumberUpdate.to_json())

# convert the object into a dict
account_number_update_dict = account_number_update_instance.to_dict()
# create an instance of AccountNumberUpdate from a dict
account_number_update_from_dict = AccountNumberUpdate.from_dict(account_number_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


