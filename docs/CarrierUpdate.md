# CarrierUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | [optional] 
**country** | **str** |  | [optional] 
**logo** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.carrier_update import CarrierUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of CarrierUpdate from a JSON string
carrier_update_instance = CarrierUpdate.from_json(json)
# print the JSON string representation of the object
print(CarrierUpdate.to_json())

# convert the object into a dict
carrier_update_dict = carrier_update_instance.to_dict()
# create an instance of CarrierUpdate from a dict
carrier_update_from_dict = CarrierUpdate.from_dict(carrier_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


