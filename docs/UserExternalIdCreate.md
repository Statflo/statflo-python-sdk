# UserExternalIdCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**user_id** | **int** |  | 
**provider** | **str** |  | 
**field_name** | **str** |  | 
**field_value** | **str** |  | 
**record_source** | **str** |  | [optional] [default to 'api']
**date_created** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.user_external_id_create import UserExternalIdCreate

# TODO update the JSON string below
json = "{}"
# create an instance of UserExternalIdCreate from a JSON string
user_external_id_create_instance = UserExternalIdCreate.from_json(json)
# print the JSON string representation of the object
print(UserExternalIdCreate.to_json())

# convert the object into a dict
user_external_id_create_dict = user_external_id_create_instance.to_dict()
# create an instance of UserExternalIdCreate from a dict
user_external_id_create_from_dict = UserExternalIdCreate.from_dict(user_external_id_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


