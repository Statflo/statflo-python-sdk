# UserMetadataCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**user_id** | **int** |  | 
**metadata** | **str** |  | [optional] 
**value** | **str** |  | [optional] 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.user_metadata_create import UserMetadataCreate

# TODO update the JSON string below
json = "{}"
# create an instance of UserMetadataCreate from a JSON string
user_metadata_create_instance = UserMetadataCreate.from_json(json)
# print the JSON string representation of the object
print(UserMetadataCreate.to_json())

# convert the object into a dict
user_metadata_create_dict = user_metadata_create_instance.to_dict()
# create an instance of UserMetadataCreate from a dict
user_metadata_create_from_dict = UserMetadataCreate.from_dict(user_metadata_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


