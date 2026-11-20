# UserTeam


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user** | [**User**](User.md) |  | 
**team** | [**Team**](Team.md) |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | 
**deleted_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.user_team import UserTeam

# TODO update the JSON string below
json = "{}"
# create an instance of UserTeam from a JSON string
user_team_instance = UserTeam.from_json(json)
# print the JSON string representation of the object
print(UserTeam.to_json())

# convert the object into a dict
user_team_dict = user_team_instance.to_dict()
# create an instance of UserTeam from a dict
user_team_from_dict = UserTeam.from_dict(user_team_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


