# VendorMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**payload** | **object** |  | 
**action** | **str** |  | [optional] 
**date_added** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.vendor_message import VendorMessage

# TODO update the JSON string below
json = "{}"
# create an instance of VendorMessage from a JSON string
vendor_message_instance = VendorMessage.from_json(json)
# print the JSON string representation of the object
print(VendorMessage.to_json())

# convert the object into a dict
vendor_message_dict = vendor_message_instance.to_dict()
# create an instance of VendorMessage from a dict
vendor_message_from_dict = VendorMessage.from_dict(vendor_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


