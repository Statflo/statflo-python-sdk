# AppointmentCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**dealer_id** | **int** |  | [optional] 
**timeline** | [**Timeline**](Timeline.md) |  | 
**timeline_id** | **int** |  | 
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
from statflo_python_sdk.models.appointment_create import AppointmentCreate

# TODO update the JSON string below
json = "{}"
# create an instance of AppointmentCreate from a JSON string
appointment_create_instance = AppointmentCreate.from_json(json)
# print the JSON string representation of the object
print(AppointmentCreate.to_json())

# convert the object into a dict
appointment_create_dict = appointment_create_instance.to_dict()
# create an instance of AppointmentCreate from a dict
appointment_create_from_dict = AppointmentCreate.from_dict(appointment_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


