# CarrierCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | [optional] 
**country** | **str** |  | [optional] 
**logo** | **str** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.carrier_create import CarrierCreate

# TODO update the JSON string below
json = "{}"
# create an instance of CarrierCreate from a JSON string
carrier_create_instance = CarrierCreate.from_json(json)
# print the JSON string representation of the object
print(CarrierCreate.to_json())

# convert the object into a dict
carrier_create_dict = carrier_create_instance.to_dict()
# create an instance of CarrierCreate from a dict
carrier_create_from_dict = CarrierCreate.from_dict(carrier_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


