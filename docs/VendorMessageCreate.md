# VendorMessageCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**payload** | **object** |  | 
**action** | **str** |  | 
**date_added** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.vendor_message_create import VendorMessageCreate

# TODO update the JSON string below
json = "{}"
# create an instance of VendorMessageCreate from a JSON string
vendor_message_create_instance = VendorMessageCreate.from_json(json)
# print the JSON string representation of the object
print(VendorMessageCreate.to_json())

# convert the object into a dict
vendor_message_create_dict = vendor_message_create_instance.to_dict()
# create an instance of VendorMessageCreate from a dict
vendor_message_create_from_dict = VendorMessageCreate.from_dict(vendor_message_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


