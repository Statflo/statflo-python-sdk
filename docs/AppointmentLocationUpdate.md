# AppointmentLocationUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**type** | **str** |  | 
**value** | **str** |  | 

## Example

```python
from statflo_python_sdk.models.appointment_location_update import AppointmentLocationUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of AppointmentLocationUpdate from a JSON string
appointment_location_update_instance = AppointmentLocationUpdate.from_json(json)
# print the JSON string representation of the object
print(AppointmentLocationUpdate.to_json())

# convert the object into a dict
appointment_location_update_dict = appointment_location_update_instance.to_dict()
# create an instance of AppointmentLocationUpdate from a dict
appointment_location_update_from_dict = AppointmentLocationUpdate.from_dict(appointment_location_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


