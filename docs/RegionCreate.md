# RegionCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 

## Example

```python
from statflo_python_sdk.models.region_create import RegionCreate

# TODO update the JSON string below
json = "{}"
# create an instance of RegionCreate from a JSON string
region_create_instance = RegionCreate.from_json(json)
# print the JSON string representation of the object
print(RegionCreate.to_json())

# convert the object into a dict
region_create_dict = region_create_instance.to_dict()
# create an instance of RegionCreate from a dict
region_create_from_dict = RegionCreate.from_dict(region_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


