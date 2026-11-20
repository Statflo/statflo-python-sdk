# LocationMetadataUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**location_id** | **int** |  | [optional] 
**metadata** | **str** |  | [optional] 
**value** | **object** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.location_metadata_update import LocationMetadataUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of LocationMetadataUpdate from a JSON string
location_metadata_update_instance = LocationMetadataUpdate.from_json(json)
# print the JSON string representation of the object
print(LocationMetadataUpdate.to_json())

# convert the object into a dict
location_metadata_update_dict = location_metadata_update_instance.to_dict()
# create an instance of LocationMetadataUpdate from a dict
location_metadata_update_from_dict = LocationMetadataUpdate.from_dict(location_metadata_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


