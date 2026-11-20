# UserExternalIdUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**user_id** | **int** |  | 
**provider** | **str** |  | 
**field_name** | **str** |  | 
**field_value** | **str** |  | 
**record_source** | **str** |  | [optional] 
**date_created** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.user_external_id_update import UserExternalIdUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of UserExternalIdUpdate from a JSON string
user_external_id_update_instance = UserExternalIdUpdate.from_json(json)
# print the JSON string representation of the object
print(UserExternalIdUpdate.to_json())

# convert the object into a dict
user_external_id_update_dict = user_external_id_update_instance.to_dict()
# create an instance of UserExternalIdUpdate from a dict
user_external_id_update_from_dict = UserExternalIdUpdate.from_dict(user_external_id_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


