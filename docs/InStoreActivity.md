# InStoreActivity


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
**user** | [**User**](User.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**account_id** | **str** |  | 
**date_added** | **datetime** |  | 
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | 
**record_source** | **str** |  | [optional] 
**record_owned** | **int** |  | [optional] [default to 1]

## Example

```python
from statflo_python_sdk.models.in_store_activity import InStoreActivity

# TODO update the JSON string below
json = "{}"
# create an instance of InStoreActivity from a JSON string
in_store_activity_instance = InStoreActivity.from_json(json)
# print the JSON string representation of the object
print(InStoreActivity.to_json())

# convert the object into a dict
in_store_activity_dict = in_store_activity_instance.to_dict()
# create an instance of InStoreActivity from a dict
in_store_activity_from_dict = InStoreActivity.from_dict(in_store_activity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


