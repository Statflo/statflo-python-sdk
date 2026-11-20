# LocationExternalId


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**dealer** | [**Dealer**](Dealer.md) |  | 
**location** | [**Location**](Location.md) |  | 
**provider** | **str** |  | [optional] [default to 'Customer']
**field_name** | **str** |  | [optional] 
**field_value** | **str** |  | 
**record_source** | **str** |  | [optional] [default to 'api']
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.location_external_id import LocationExternalId

# TODO update the JSON string below
json = "{}"
# create an instance of LocationExternalId from a JSON string
location_external_id_instance = LocationExternalId.from_json(json)
# print the JSON string representation of the object
print(LocationExternalId.to_json())

# convert the object into a dict
location_external_id_dict = location_external_id_instance.to_dict()
# create an instance of LocationExternalId from a dict
location_external_id_from_dict = LocationExternalId.from_dict(location_external_id_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


