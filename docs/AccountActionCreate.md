# AccountActionCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_content** | **object** |  | [optional] 
**action_taken** | **str** |  | [optional] [default to 'Reassignment']
**message_to** | **str** |  | [optional] 
**message_from** | **str** |  | [optional] 
**id** | **int** |  | 
**type** | **int** |  | 
**account_id** | **str** |  | 
**date_added** | **datetime** |  | 
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | 
**record_source** | **str** |  | [optional] 
**record_owned** | **int** |  | [optional] [default to 1]

## Example

```python
from statflo_python_sdk.models.account_action_create import AccountActionCreate

# TODO update the JSON string below
json = "{}"
# create an instance of AccountActionCreate from a JSON string
account_action_create_instance = AccountActionCreate.from_json(json)
# print the JSON string representation of the object
print(AccountActionCreate.to_json())

# convert the object into a dict
account_action_create_dict = account_action_create_instance.to_dict()
# create an instance of AccountActionCreate from a dict
account_action_create_from_dict = AccountActionCreate.from_dict(account_action_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


