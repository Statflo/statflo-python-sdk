# DistrictCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**region_id** | **int** |  | 

## Example

```python
from statflo_python_sdk.models.district_create import DistrictCreate

# TODO update the JSON string below
json = "{}"
# create an instance of DistrictCreate from a JSON string
district_create_instance = DistrictCreate.from_json(json)
# print the JSON string representation of the object
print(DistrictCreate.to_json())

# convert the object into a dict
district_create_dict = district_create_instance.to_dict()
# create an instance of DistrictCreate from a dict
district_create_from_dict = DistrictCreate.from_dict(district_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


