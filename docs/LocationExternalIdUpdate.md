# LocationExternalIdUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**location_id** | **int** |  | [optional] 
**provider** | **str** |  | [optional] 
**field_name** | **str** |  | [optional] 
**field_value** | **str** |  | 
**record_source** | **str** |  | [optional] 
**date_created** | **datetime** |  | 
**date_updated** | **datetime** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.location_external_id_update import LocationExternalIdUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of LocationExternalIdUpdate from a JSON string
location_external_id_update_instance = LocationExternalIdUpdate.from_json(json)
# print the JSON string representation of the object
print(LocationExternalIdUpdate.to_json())

# convert the object into a dict
location_external_id_update_dict = location_external_id_update_instance.to_dict()
# create an instance of LocationExternalIdUpdate from a dict
location_external_id_update_from_dict = LocationExternalIdUpdate.from_dict(location_external_id_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


