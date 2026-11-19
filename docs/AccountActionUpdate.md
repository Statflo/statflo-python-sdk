# AccountActionUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_content** | **object** |  | [optional] 
**action_taken** | **str** |  | [optional] 
**message_to** | **str** |  | [optional] 
**message_from** | **str** |  | [optional] 
**id** | **int** |  | 
**type** | **int** |  | 
**account_id** | **str** |  | 
**date_added** | **datetime** |  | 
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | 
**record_source** | **str** |  | [optional] 
**record_owned** | **int** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.account_action_update import AccountActionUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of AccountActionUpdate from a JSON string
account_action_update_instance = AccountActionUpdate.from_json(json)
# print the JSON string representation of the object
print(AccountActionUpdate.to_json())

# convert the object into a dict
account_action_update_dict = account_action_update_instance.to_dict()
# create an instance of AccountActionUpdate from a dict
account_action_update_from_dict = AccountActionUpdate.from_dict(account_action_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


