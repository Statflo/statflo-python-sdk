# BulkMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**user** | [**User**](User.md) |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**template** | [**MessageTemplate**](MessageTemplate.md) |  | 
**campaign** | [**Campaign**](Campaign.md) |  | 
**location** | [**Location**](Location.md) |  | 
**delivery_status** | **str** |  | [optional] [default to 'sending']
**provider** | **str** |  | [optional] [default to 'twilio']
**content** | **str** |  | [optional] 
**date_added** | **datetime** |  | 

## Example

```python
from statflo_python_sdk.models.bulk_message import BulkMessage

# TODO update the JSON string below
json = "{}"
# create an instance of BulkMessage from a JSON string
bulk_message_instance = BulkMessage.from_json(json)
# print the JSON string representation of the object
print(BulkMessage.to_json())

# convert the object into a dict
bulk_message_dict = bulk_message_instance.to_dict()
# create an instance of BulkMessage from a dict
bulk_message_from_dict = BulkMessage.from_dict(bulk_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


