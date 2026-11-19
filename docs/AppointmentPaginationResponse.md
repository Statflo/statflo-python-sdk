# AppointmentPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[Appointment]**](Appointment.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.appointment_pagination_response import AppointmentPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppointmentPaginationResponse from a JSON string
appointment_pagination_response_instance = AppointmentPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(AppointmentPaginationResponse.to_json())

# convert the object into a dict
appointment_pagination_response_dict = appointment_pagination_response_instance.to_dict()
# create an instance of AppointmentPaginationResponse from a dict
appointment_pagination_response_from_dict = AppointmentPaginationResponse.from_dict(appointment_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


