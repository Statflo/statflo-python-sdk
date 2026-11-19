# AppointmentLocationCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**type** | **str** |  | 
**value** | **str** |  | 

## Example

```python
from statflo_python_sdk.models.appointment_location_create import AppointmentLocationCreate

# TODO update the JSON string below
json = "{}"
# create an instance of AppointmentLocationCreate from a JSON string
appointment_location_create_instance = AppointmentLocationCreate.from_json(json)
# print the JSON string representation of the object
print(AppointmentLocationCreate.to_json())

# convert the object into a dict
appointment_location_create_dict = appointment_location_create_instance.to_dict()
# create an instance of AppointmentLocationCreate from a dict
appointment_location_create_from_dict = AppointmentLocationCreate.from_dict(appointment_location_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


