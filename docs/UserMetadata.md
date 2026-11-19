# UserMetadata


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**user** | [**User**](User.md) |  | 
**metadata** | **str** |  | [optional] 
**value** | **str** |  | [optional] 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.user_metadata import UserMetadata

# TODO update the JSON string below
json = "{}"
# create an instance of UserMetadata from a JSON string
user_metadata_instance = UserMetadata.from_json(json)
# print the JSON string representation of the object
print(UserMetadata.to_json())

# convert the object into a dict
user_metadata_dict = user_metadata_instance.to_dict()
# create an instance of UserMetadata from a dict
user_metadata_from_dict = UserMetadata.from_dict(user_metadata_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


