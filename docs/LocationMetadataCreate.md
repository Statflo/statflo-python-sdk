# LocationMetadataCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**location_id** | **int** |  | 
**metadata** | **str** |  | 
**value** | **object** |  | [optional] 

## Example

```python
from statflo_python_sdk.models.location_metadata_create import LocationMetadataCreate

# TODO update the JSON string below
json = "{}"
# create an instance of LocationMetadataCreate from a JSON string
location_metadata_create_instance = LocationMetadataCreate.from_json(json)
# print the JSON string representation of the object
print(LocationMetadataCreate.to_json())

# convert the object into a dict
location_metadata_create_dict = location_metadata_create_instance.to_dict()
# create an instance of LocationMetadataCreate from a dict
location_metadata_create_from_dict = LocationMetadataCreate.from_dict(location_metadata_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


