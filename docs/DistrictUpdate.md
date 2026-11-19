# DistrictUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**region_id** | **int** |  | 

## Example

```python
from statflo_python_sdk.models.district_update import DistrictUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of DistrictUpdate from a JSON string
district_update_instance = DistrictUpdate.from_json(json)
# print the JSON string representation of the object
print(DistrictUpdate.to_json())

# convert the object into a dict
district_update_dict = district_update_instance.to_dict()
# create an instance of DistrictUpdate from a dict
district_update_from_dict = DistrictUpdate.from_dict(district_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


