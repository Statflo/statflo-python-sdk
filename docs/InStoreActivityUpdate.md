# InStoreActivityUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_to** | **str** |  | [optional] 
**message_from** | **str** |  | [optional] 
**subject** | **str** |  | [optional] 
**action_taken** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**next_steps** | **str** |  | [optional] 
**next_date** | **datetime** |  | [optional] 
**outcome_reason** | **str** |  | [optional] 
**outcome_location** | **str** |  | [optional] 
**id** | **int** |  | 
**type** | **int** |  | 
**account_id** | **str** |  | 
**date_added** | **datetime** |  | 
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | 
**record_source** | **str** |  | [optional] 
**record_owned** | **int** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.in_store_activity_update import InStoreActivityUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of InStoreActivityUpdate from a JSON string
in_store_activity_update_instance = InStoreActivityUpdate.from_json(json)
# print the JSON string representation of the object
print(InStoreActivityUpdate.to_json())

# convert the object into a dict
in_store_activity_update_dict = in_store_activity_update_instance.to_dict()
# create an instance of InStoreActivityUpdate from a dict
in_store_activity_update_from_dict = InStoreActivityUpdate.from_dict(in_store_activity_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


