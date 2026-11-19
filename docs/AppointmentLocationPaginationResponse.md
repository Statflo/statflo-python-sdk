# AppointmentLocationPaginationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[AppointmentLocation]**](AppointmentLocation.md) |  | [optional] 
**pagination** | [**Pagination**](Pagination.md) |  | [optional] 
**aggregations** | **Dict[str, object]** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.appointment_location_pagination_response import AppointmentLocationPaginationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AppointmentLocationPaginationResponse from a JSON string
appointment_location_pagination_response_instance = AppointmentLocationPaginationResponse.from_json(json)
# print the JSON string representation of the object
print(AppointmentLocationPaginationResponse.to_json())

# convert the object into a dict
appointment_location_pagination_response_dict = appointment_location_pagination_response_instance.to_dict()
# create an instance of AppointmentLocationPaginationResponse from a dict
appointment_location_pagination_response_from_dict = AppointmentLocationPaginationResponse.from_dict(appointment_location_pagination_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


