# LocationExternalIdCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**location_id** | **int** |  | 
**provider** | **str** |  | [optional] [default to 'Customer']
**field_name** | **str** |  | 
**field_value** | **str** |  | 
**record_source** | **str** |  | [optional] [default to 'api']
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.location_external_id_create import LocationExternalIdCreate

# TODO update the JSON string below
json = "{}"
# create an instance of LocationExternalIdCreate from a JSON string
location_external_id_create_instance = LocationExternalIdCreate.from_json(json)
# print the JSON string representation of the object
print(LocationExternalIdCreate.to_json())

# convert the object into a dict
location_external_id_create_dict = location_external_id_create_instance.to_dict()
# create an instance of LocationExternalIdCreate from a dict
location_external_id_create_from_dict = LocationExternalIdCreate.from_dict(location_external_id_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


