# Appointment


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**timeline** | [**Timeline**](Timeline.md) |  | 
**account_id** | **str** |  | 
**user** | [**User**](User.md) |  | 
**user_id** | **int** |  | 
**date_from** | **datetime** |  | 
**date_to** | **datetime** |  | 
**location** | [**AppointmentLocation**](AppointmentLocation.md) |  | 
**location_id** | **str** |  | 
**note** | **str** |  | 
**date_created** | **datetime** |  | 
**notified_at** | **datetime** |  | [optional] 
**confirmed_at** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.appointment import Appointment

# TODO update the JSON string below
json = "{}"
# create an instance of Appointment from a JSON string
appointment_instance = Appointment.from_json(json)
# print the JSON string representation of the object
print(Appointment.to_json())

# convert the object into a dict
appointment_dict = appointment_instance.to_dict()
# create an instance of Appointment from a dict
appointment_from_dict = Appointment.from_dict(appointment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


