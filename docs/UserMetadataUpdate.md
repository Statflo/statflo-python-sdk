# UserMetadataUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**user_id** | **int** |  | [optional] 
**metadata** | **str** |  | [optional] 
**value** | **str** |  | [optional] 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.user_metadata_update import UserMetadataUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of UserMetadataUpdate from a JSON string
user_metadata_update_instance = UserMetadataUpdate.from_json(json)
# print the JSON string representation of the object
print(UserMetadataUpdate.to_json())

# convert the object into a dict
user_metadata_update_dict = user_metadata_update_instance.to_dict()
# create an instance of UserMetadataUpdate from a dict
user_metadata_update_from_dict = UserMetadataUpdate.from_dict(user_metadata_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


