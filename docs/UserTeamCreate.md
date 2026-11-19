# UserTeamCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **int** |  | 
**team_id** | **int** |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | 
**deleted_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.user_team_create import UserTeamCreate

# TODO update the JSON string below
json = "{}"
# create an instance of UserTeamCreate from a JSON string
user_team_create_instance = UserTeamCreate.from_json(json)
# print the JSON string representation of the object
print(UserTeamCreate.to_json())

# convert the object into a dict
user_team_create_dict = user_team_create_instance.to_dict()
# create an instance of UserTeamCreate from a dict
user_team_create_from_dict = UserTeamCreate.from_dict(user_team_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


