# DealerCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**country_code** | **str** |  | 
**calendar_format** | **int** |  | [optional] [default to 0]
**website** | **str** |  | [optional] 
**address_line1** | **str** |  | [optional] 
**address_line2** | **str** |  | [optional] 
**city** | **str** |  | [optional] 
**province** | **str** |  | [optional] 
**postal_code** | **str** |  | [optional] 
**features** | **List[int]** |  | 

## Example

```python
from statflo_python_sdk.models.dealer_create import DealerCreate

# TODO update the JSON string below
json = "{}"
# create an instance of DealerCreate from a JSON string
dealer_create_instance = DealerCreate.from_json(json)
# print the JSON string representation of the object
print(DealerCreate.to_json())

# convert the object into a dict
dealer_create_dict = dealer_create_instance.to_dict()
# create an instance of DealerCreate from a dict
dealer_create_from_dict = DealerCreate.from_dict(dealer_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


