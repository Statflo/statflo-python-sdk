# AppointmentLocation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**type** | **str** |  | 
**value** | **str** |  | 

## Example

```python
from statflo_python_sdk.models.appointment_location import AppointmentLocation

# TODO update the JSON string below
json = "{}"
# create an instance of AppointmentLocation from a JSON string
appointment_location_instance = AppointmentLocation.from_json(json)
# print the JSON string representation of the object
print(AppointmentLocation.to_json())

# convert the object into a dict
appointment_location_dict = appointment_location_instance.to_dict()
# create an instance of AppointmentLocation from a dict
appointment_location_from_dict = AppointmentLocation.from_dict(appointment_location_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


