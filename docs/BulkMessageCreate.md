# BulkMessageCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**user_id** | **int** |  | 
**template_id** | **str** |  | 
**campaign_id** | **int** |  | 
**location_id** | **int** |  | 
**delivery_status** | **str** |  | [optional] [default to 'sending']
**provider** | **str** |  | [optional] [default to 'twilio']
**content** | **str** |  | [optional] 
**date_added** | **datetime** |  | 

## Example

```python
from statflo_python_sdk.models.bulk_message_create import BulkMessageCreate

# TODO update the JSON string below
json = "{}"
# create an instance of BulkMessageCreate from a JSON string
bulk_message_create_instance = BulkMessageCreate.from_json(json)
# print the JSON string representation of the object
print(BulkMessageCreate.to_json())

# convert the object into a dict
bulk_message_create_dict = bulk_message_create_instance.to_dict()
# create an instance of BulkMessageCreate from a dict
bulk_message_create_from_dict = BulkMessageCreate.from_dict(bulk_message_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


