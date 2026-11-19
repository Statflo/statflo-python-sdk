# TeamAccessible


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**team** | [**Team**](Team.md) |  | 

## Example

```python
from statflo_python_sdk.models.team_accessible import TeamAccessible

# TODO update the JSON string below
json = "{}"
# create an instance of TeamAccessible from a JSON string
team_accessible_instance = TeamAccessible.from_json(json)
# print the JSON string representation of the object
print(TeamAccessible.to_json())

# convert the object into a dict
team_accessible_dict = team_accessible_instance.to_dict()
# create an instance of TeamAccessible from a dict
team_accessible_from_dict = TeamAccessible.from_dict(team_accessible_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


