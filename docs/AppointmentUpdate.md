# AppointmentUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**dealer_id** | **int** |  | [optional] 
**timeline_id** | **int** |  | [optional] 
**account_id** | **str** |  | 
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
from statflo_python_sdk.models.appointment_update import AppointmentUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of AppointmentUpdate from a JSON string
appointment_update_instance = AppointmentUpdate.from_json(json)
# print the JSON string representation of the object
print(AppointmentUpdate.to_json())

# convert the object into a dict
appointment_update_dict = appointment_update_instance.to_dict()
# create an instance of AppointmentUpdate from a dict
appointment_update_from_dict = AppointmentUpdate.from_dict(appointment_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


