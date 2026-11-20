# BulkMessageUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**user_id** | **int** |  | 
**template_id** | **str** |  | 
**campaign_id** | **int** |  | 
**location_id** | **int** |  | 
**delivery_status** | **str** |  | [optional] 
**provider** | **str** |  | [optional] 
**content** | **str** |  | [optional] 
**date_added** | **datetime** |  | 

## Example

```python
from statflo_python_sdk.models.bulk_message_update import BulkMessageUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of BulkMessageUpdate from a JSON string
bulk_message_update_instance = BulkMessageUpdate.from_json(json)
# print the JSON string representation of the object
print(BulkMessageUpdate.to_json())

# convert the object into a dict
bulk_message_update_dict = bulk_message_update_instance.to_dict()
# create an instance of BulkMessageUpdate from a dict
bulk_message_update_from_dict = BulkMessageUpdate.from_dict(bulk_message_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


