# DealerUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**country_code** | **str** |  | 
**calendar_format** | **int** |  | [optional] 
**website** | **str** |  | [optional] 
**address_line1** | **str** |  | [optional] 
**address_line2** | **str** |  | [optional] 
**city** | **str** |  | [optional] 
**province** | **str** |  | [optional] 
**postal_code** | **str** |  | [optional] 
**features** | **List[int]** |  | 

## Example

```python
from statflo_python_sdk.models.dealer_update import DealerUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of DealerUpdate from a JSON string
dealer_update_instance = DealerUpdate.from_json(json)
# print the JSON string representation of the object
print(DealerUpdate.to_json())

# convert the object into a dict
dealer_update_dict = dealer_update_instance.to_dict()
# create an instance of DealerUpdate from a dict
dealer_update_from_dict = DealerUpdate.from_dict(dealer_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


