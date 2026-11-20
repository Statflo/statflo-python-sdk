# ReassignRep


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**user** | [**User**](User.md) |  | 
**new_external_user_id** | **str** |  | [optional] 
**old_external_user_id** | **str** |  | [optional] 
**new_external_location_id** | **str** |  | [optional] 
**old_external_location_id** | **str** |  | [optional] 
**account_name** | **str** |  | 
**account_id** | **str** |  | 
**date_changed** | **datetime** |  | 
**reason** | **str** |  | [optional] [default to 'api']
**old_ban** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.reassign_rep import ReassignRep

# TODO update the JSON string below
json = "{}"
# create an instance of ReassignRep from a JSON string
reassign_rep_instance = ReassignRep.from_json(json)
# print the JSON string representation of the object
print(ReassignRep.to_json())

# convert the object into a dict
reassign_rep_dict = reassign_rep_instance.to_dict()
# create an instance of ReassignRep from a dict
reassign_rep_from_dict = ReassignRep.from_dict(reassign_rep_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


