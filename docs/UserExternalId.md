# UserExternalId


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**user** | [**User**](User.md) |  | 
**provider** | **str** |  | 
**field_name** | **str** |  | 
**field_value** | **str** |  | 
**record_source** | **str** |  | [optional] [default to 'api']
**date_created** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.user_external_id import UserExternalId

# TODO update the JSON string below
json = "{}"
# create an instance of UserExternalId from a JSON string
user_external_id_instance = UserExternalId.from_json(json)
# print the JSON string representation of the object
print(UserExternalId.to_json())

# convert the object into a dict
user_external_id_dict = user_external_id_instance.to_dict()
# create an instance of UserExternalId from a dict
user_external_id_from_dict = UserExternalId.from_dict(user_external_id_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


