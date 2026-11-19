# AccountAction


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_content** | **object** |  | [optional] 
**action_taken** | **str** |  | [optional] [default to 'Reassignment']
**message_to** | **str** |  | [optional] 
**message_from** | **str** |  | [optional] 
**id** | **int** |  | 
**type** | **int** |  | 
**user** | [**User**](User.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**account_id** | **str** |  | 
**date_added** | **datetime** |  | 
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | 
**record_source** | **str** |  | [optional] 
**record_owned** | **int** |  | [optional] [default to 1]

## Example

```python
from statflo_python_sdk.models.account_action import AccountAction

# TODO update the JSON string below
json = "{}"
# create an instance of AccountAction from a JSON string
account_action_instance = AccountAction.from_json(json)
# print the JSON string representation of the object
print(AccountAction.to_json())

# convert the object into a dict
account_action_dict = account_action_instance.to_dict()
# create an instance of AccountAction from a dict
account_action_from_dict = AccountAction.from_dict(account_action_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


