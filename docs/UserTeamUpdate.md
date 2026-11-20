# UserTeamUpdate


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
from statflo_python_sdk.models.user_team_update import UserTeamUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of UserTeamUpdate from a JSON string
user_team_update_instance = UserTeamUpdate.from_json(json)
# print the JSON string representation of the object
print(UserTeamUpdate.to_json())

# convert the object into a dict
user_team_update_dict = user_team_update_instance.to_dict()
# create an instance of UserTeamUpdate from a dict
user_team_update_from_dict = UserTeamUpdate.from_dict(user_team_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


